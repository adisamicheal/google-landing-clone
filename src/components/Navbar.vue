<template>
  <div>
      <nav>
          <div class="nav_items">
              <ul>
                  <li><a href="" class="nav_link">Gmail</a></li>
                  <li><a href="" class="nav_link">Images</a></li>
                  <li><a href=""><img src="@/assets/grid.svg" alt="menu" class="grid_icon"></a></li>
                  <li><a href=""><img src="https://lh3.googleusercontent.com/ogw/ADGmqu-JBmRSECfCjISsSOSrBposK6F9J86TgFKPlzwQ=s64-c-mo" alt="account_owner" class="account_owner"></a></li>
              </ul>
          </div>
      </nav>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
nav {
    padding-top: 20px;
}
.nav_items {
    float: right;
}
.nav_items >ul {
    display: flex;
    align-items: center;
    justify-content: space-between;
    list-style: none;
    padding: 0 32px;
    font-size: 13px;
}
.nav_items >ul>li {
    margin-left: 20px;
}
.nav_link {
    text-decoration: none;
    color: rgba(0,0,0,0.87);
}
.nav_link:hover {
    opacity: .85;
    text-decoration: underline;
}
.grid_icon {
    height: 15px;
    opacity: 0.5;
}
.grid_icon:hover {
    opacity: 1;
}
.account_owner {
    border-radius: 50px;
    height: 30px;
}
</style>
