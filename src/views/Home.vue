<template>
  <div class="home">
    <div class="nav">
      <Navbar />
    </div>
    <div class="container">
      <div class="main_content">
        <img src="https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png" alt="google logo" class="google_logo">
        <div class="search_box">
          <img src="@/assets/search.svg" alt="search icon" class="search_icon">
          <input type="text" class="search_input">
          <img src="@/assets/microphone.svg" alt="microphone icon" class="microphone_icon">
        </div>
        <div class="buttons">
          <button>Google Search</button>
          <button>I'm Feeling Lucky</button>
        </div>
        <div class="language">
          <ul>
            <li>Google offered in: </li>
            <li><a href="https://www.google.com/setprefs?sig=0_5nJgMhr8VadvBrZE4JenWvOuKAg%3D&hl=ha&source=homepage&sa=X&ved=0ahUKEwirooH-4OrrAhXhx4UKHfZmBBAQ2ZgBCA8">Hausa</a></li>
            <li><a href="https://www.google.com/setprefs?sig=0_5nJgMhr8VadvBrZE4JenWvOuKAg%3D&hl=ig&source=homepage&sa=X&ved=0ahUKEwirooH-4OrrAhXhx4UKHfZmBBAQ2ZgBCBA">Igbo</a></li>
            <li><a href="https://www.google.com/setprefs?sig=0_5nJgMhr8VadvBrZE4JenWvOuKAg%3D&hl=yo&source=homepage&sa=X&ved=0ahUKEwirooH-4OrrAhXhx4UKHfZmBBAQ2ZgBCBE">Èdè Yorùbá</a></li>
            <li><a href="https://www.google.com/setprefs?sig=0_5nJgMhr8VadvBrZE4JenWvOuKAg%3D&hl=pcm&source=homepage&sa=X&ved=0ahUKEwirooH-4OrrAhXhx4UKHfZmBBAQ2ZgBCBI">Nigerian Pidgin</a></li>
          </ul>
        </div>
      </div>
    </div>
    <div class="footer">
      <Footer />
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import  Navbar  from "@/components/Navbar";
import  Footer  from "@/components/Footer";

export default {
  name: 'Home',
  components: {
    Navbar,
    Footer
  }
}
</script>

<style scoped>
.home {
  display: flex;
  flex-direction: column;
}
.container {
  height: 81vh;
}
.main_content {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-top: 150px;
}
.google_logo {
  height: 100px;
}
.search_box {
  border-radius: 30px;
  height: 50px;
  width: 45%;
  border: 1px solid #dfe1e5;
  box-shadow: none;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 0 20px;
  margin-top: 30px;
}
.search_box:hover {
  box-shadow: 0 1px 6px 0 rgba(32,33,36,0.28);
  border-color: rgba(223,225,229,0);
}
.search_icon {
  width: 15px;
}
.search_input {
  width: 90%;
  border: none;
  padding: 0 20px;
}
input:focus{
  outline: none;
}
.microphone_icon {
  width: 20px;
}
.buttons {
  padding-top: 20px;
}
.buttons > button {
  background-color: #f2f2f2;
  border: 1px solid #f2f2f2;
  border-radius: 4px;
  color: #5F6368;
  font-family: arial,sans-serif;
  font-size: 14px;
  margin: 11px 4px;
  padding: 0 16px;
  line-height: 27px;
  height: 36px;
  min-width: 54px;
  text-align: center;
  cursor: pointer;
  user-select: none;
}
.buttons > button:hover {
  box-shadow: 0 1px 1px rgba(0,0,0,0.1);
  background-image: -webkit-linear-gradient(top,#f8f8f8,#f1f1f1);
  background-color: #f8f8f8;
  border: 1px solid #c6c6c6;
  color: #222;
}
.language {
  line-height: 28px;
  font-size: small;
  display: flex;
  align-items: center;
  margin-top: 20px;
}
.language>ul {
  list-style: none;
  display: flex;
  align-items: center;
  padding-left: 0;
}
.language>ul>li{
  margin-left: 10px;
}
.language>ul>li>a {
  color: #1a0dab;
  text-decoration: none;
}
.language>ul>li>a:hover {
  text-decoration: underline;
}
.footer {
  margin-top: auto;
}
@media screen and (max-width: 768px) {
  .search_box {
    width: 80%;
  }
}
</style>
