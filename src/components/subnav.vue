<template>
  <section id="subnav1">
    <v-layout id="subnav">
      <div class="logo">
        <a href="#"
          ><img
            id="logo2"
            height="100px"
            src="http://medilab.co.ke/wp-content/uploads/2017/04/logo-medilab.jpg"
            alt=""
            srcset=""
        /></a>
      </div>
      <nav class="navbar navbar-expand-lg navbar-light">
        <div class="container">
          <div class="collapse navbar-collapse" id="navbarSupportedContent">
            <ul class="navbar-nav ml-auto">
              <li class="nav-item">
                <a class="nav-link" href="/">Home</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" href="products">Products</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" href="/Services">services</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" href="/about">About</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" href="contact.html">Contact</a>
              </li>
            </ul>
          </div>
        </div>
      </nav>
      <!-- <v-flex class="subnav-content">
        <div class="nav-content">
          <div class="navlinks"><a href="#">Home</a></div>
          <div class="navlinks"><a href="#"></a></div>
          <div class="navlinks"><a href="#">Services</a></div>
          <div class="navlinks"><a href="#">About Us</a></div>
          <div class="navlinks"><a href="#">Contact Us</a></div>
        </div>
      </v-flex> -->
    </v-layout>
  </section>
</template>
<script>
export default {
  name: "subnav"
};
</script>
<style scoped>
.container {
  position: relative;
  left: 400px;
  width: 600px;
}
#logo {
  padding: 40px;
  width: 80px;
  height: 60px;
  position: relative;
  left: -130px;
}
#navbarSupportedContent {
  padding: 0px 60px;
}
#logo2 {
  position: relative;
  left: -300px;
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
#menu {
  display: none;
}
.nav-item {
  color: #fff;
  padding: 10px 20px;
  position: relative;
  text-align: center;
  border-bottom: 3px solid transparent;
  display: flex;
  left: -100px;

  padding: auto;
}
.nav-link {
  color: blue;
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
.nav-link.active,
a:hover,
.nav-link:hover {
  color: #00aeff;
  border-bottom-color: #00aeff;
  transition: width 2.4s linear;
  transition-property: border-bottom;
}
@media screen and (max-width: 1150px) {
  .nav-link {
    display: none;
  }
  .container {
    position: relative;
    left: 500px;
  }
  .nav-content {
    display: none;
  }
  #logo2 {
    position: relative;
    left: -120px;
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
@media only screen and (max-width: 767px) {
  .navbar-nav.ml-auto {
    background: rgba(0, 0, 0, 0.5);
  }

  .navbar-nav a {
    font-size: 14px;
    font-weight: normal;
  }
}
@media screen and (max-width: 670px) {
  .nav-link {
    display: none;
  }
  .container {
    position: relative;
    left: 500px;
  }
  .nav-content {
    display: none;
  }
  #logo2 {
    position: relative;
    left: -120px;
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
@media screen and (max-width: 450px) {
  .nav-link {
    display: none;
  }
  .nav-content {
    display: none;
  }
  .container {
    position: relative;
    right: 0px;
    transition: all 1s ease;
  }
  #logo2 {
    position: relative;
    left: 64px;
    height: 60px;
    transition: all 1s ease;
  }
  #menu {
    position: relative;
    left: 300px;
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
  .small {
    right: 0px;
    position: absolute;
  }
}
</style>
