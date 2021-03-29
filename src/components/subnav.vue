<template>
  <section id="subnav1">
    <v-layout id="subnav">
      <div class="logo">
        <a href="#"
          ><img
            id="logo2"
            height="90px"
            src="http://medilab.co.ke/wp-content/uploads/2017/04/logo-medilab.jpg"
            alt=""
            srcset=""
        /></a>
      </div>
      <div class="small">
        <i class="fas fa-bars"></i>
      </div>
      <v-flex class="subnav-content">
        <div class="nav-content">
          <div class="navlinks"><a href="#">Home</a></div>
          <div class="navlinks"><a href="#">Products</a></div>
          <div class="navlinks"><a href="#">Services</a></div>
          <div class="navlinks"><a href="#">About Us</a></div>
          <div class="navlinks"><a href="#">Contact Us</a></div>
        </div>
      </v-flex>
    </v-layout>
  </section>
</template>
<script>
export default {
  name: "subnav"
};
</script>
<style scoped>
#logo {
  padding: 40px;
  width: 80px;
  height: 60px;
  position: relative;
  left: 30px;
}
#logo2 {
  position: relative;
  left: 100px;
}
#subnav {
  width: 100vw;
  background: white;
  height: 120px;
  display: flex;
  align-items: flex-end;
  position: relative;
  right: 0px;
  justify-content: center;
}
.subnav-content {
  color: #fff;
  padding: 10px 35px;
  position: relative;
  text-align: center;
  border-bottom: 3px solid transparent;
  display: flex;

  margin-right: 0;
  right: 0px;
  margin-left: 500px;
}
.nav-content {
  color: #fff;
  padding: 10px 20px;
  position: relative;
  text-align: center;
  border-bottom: 3px solid transparent;
  display: flex;
  left: 0px;

  padding: auto;
}
.navlinks {
  color: #fff;
  padding: 1px 20px;
  position: relative;
  text-align: center;
  border-bottom: 1px solid transparent;
  display: flex;
  float: right;
  transition: width 4.4s;
}
a {
  text-decoration: none;
  color: blue;
}
.navlinks.active,
a:hover,
.navlinks:hover {
  color: #00aeff;
  border-bottom-color: #00aeff;
  transition: width 2.4s linear;
  transition-property: border-bottom;
}
@media screen and (max-width: 1150px) {
  .navlinks {
    display: none;
  }
  .nav-content {
    display: none;
  }
  #logo2 {
    position: relative;
    left: 20px;
    height: 80px;
  }
  #subnav {
  max-width: 100%;
  background: white;
  height: 90px;
  display: flex;
  align-items: flex-end;
  position: relative;
  right: 0px;
  left: 0px;
  justify-content: center;
}
}
@media screen and (max-width: 670px) {
  .navlinks {
    display: none;
  }
  .nav-content {
    display: none;
  }
  #logo2 {
    position: relative;
    margin-left: 230px;
    height: 60px;
    transition: all 1s ease;
  }
  #subnav {
  max-width: 100%;
  background: white;
  height: 90px;
  display: flex;
  align-items: flex-end;
  position: relative;
  right: 0px;
  left: 0px;
  justify-content: center;
}
}


</style>
