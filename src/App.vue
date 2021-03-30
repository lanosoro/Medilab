<template>
  <div id="app">
    <header>
      <mobinav id="mobinav" />
    </header>
    <!-- <the-desktop-nav id="desktop-nav" class="d-sm-none d-md-flex" /> -->

    <subnav id="subnav" />
    <div class="view-container">
      <router-view />
    </div>

    <!-- <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div> -->
    
      <topfooter />
 
    
  </div>
</template>
<script>
// import TheDesktopNav from "./components/TheDesktopNav.vue";
import mobinav from "./components/mobinav";
import Subnav from "./components/subnav.vue";
import topfooter from "./components/footer2";
export default {
  components: {
    // TheDesktopNav,
    mobinav,
    Subnav,
    topfooter
  }
};
</script>

<style scoped>
header {
  width: 100vw;
  padding: 8px;
  position: relative;
  left: 0;
  right: 0;
  background: #28b6e7;
}

#topfooter {
  position: relative;
  left: 0;
  right: 0;
  padding: 10px 50px;
  background: #0074a5;
  width: 100vw;
  height: 400px;
}
.view-container {
  width: 100vw;
  padding: 0px;
  margin-left: 0vw;
  box-sizing: border-box;
  min-height: 100vh;
  overflow: none;
  position: relative;
}
#desktop-nav {
  display: none;
}
#mobinav {
}
@media screen and (max-width: 950px) {
  #desktop-nav {
    display: none;
  }
  .view-container {
    width: 100%;
    margin-left: 0;

    font-size: 11px;
  }
  #mobinav {
    display: flex;
    flex-direction: column;
    width: 100%;
  }
  #subnav {
    display: flex;
    flex-direction: column;
    width: 100%;
    margin-left: 0;
  }
  #topfooter {
    bottom: 0;
    position: relative;
  }
  #bottomfooter{
    bottom: 0px;
  }
}
</style>
