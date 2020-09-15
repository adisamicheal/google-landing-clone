<template>
  <div class="foot">
      <div>
          <p>Nigeria</p>
      </div>
      <div class="links">
          <div>
              <ul>
                  <li><a href="">Advertising</a></li>
                  <li><a href="">Business</a></li>
                  <li><a href="">About</a></li>
                  <li><a href="">How Search works</a></li>
              </ul>
          </div>
           <div>
              <ul>
                  <li><a href="">Privacy</a></li>
                  <li><a href="">Terms</a></li>
                  <li><a href="">Settings</a></li>
              </ul>
          </div>
      </div>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.foot {
    background: #f2f2f2;
    padding: 20px 0;
}
p {
    font-size: 14px;
    color: #5f6368;
    padding-left: 20px;
}
.links {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding-top: 20px;
    padding-right: 20px;
}
ul {
    list-style: none;
    display: flex;
}
ul>li>a {
    text-decoration: none;
    font-size: 14px;
    color: #5f6368;
}
ul>li>a:hover {
    text-decoration: underline;
}
ul>li {
    padding-left: 20px;
}
</style>