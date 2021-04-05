<template>
  <v-layout fluid class="pa-0" fill-width id="container">
    <nav
      flat
      style="background:white; z-index:200; width:100%; height:20px; position:relative; left:0px; box-shadow: 0px 2px 2px rgba(0,0,0,0.1);"
      id="nav"
    >
      <v-icon>
        mdi-account
      </v-icon>
      <v-avatar
        style="position:absolute; left:15px; bottom:10px;"
        :color="$vuetify.breakpoint.smAndDown ? 'grey darken-1' : 'transparent'"
        size="42"
      >
        <v-img
          width="100%"
          src="https://mpng.subpng.com/20180622/uz/kisspng-facebook-inc-social-media-computer-icons-social-share-facebook-5b2d58d7da0246.193322341529698519893.jpg"
        ></v-img>
      </v-avatar>
      <div class="dropdown-list">
        <div class="dropdown-list__item">
          <a
            style="text-decoration:none; color:black; font-weight:700; padding:3px 8px; "
            >logOut</a
          >
        </div>
      </div>
    </nav>
    <v-card id="main">
      <div class="midnav" style="">
        <div class="navcon"><a href="#">Posts</a></div>
        <div class="navcon"><a href="#">About</a></div>
        <div class="navcon"><a href="#">Friends</a></div>
        <div class="navcon"><a href="#">Photos</a></div>
        <div class="navcon"><a href="#">more</a></div>
      </div>
      <div flat id="main2">
        <v-avatar size="160px" style="z-index:10000;" id="dpic">
          <v-img
            width="100%"
            src="data:image/png;base64,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"
          ></v-img>
        </v-avatar>
      </div>
      <div class="line"></div>
      <div class="line2"></div>
    </v-card>

    <v-card elevation="5px" id="content1"> <webDropdownVue /> </v-card>
    <v-card id="content2">
      <v-avatar size="45px" style="z-index:10000;" id="dpic2">
        <v-img
          width="100%"
          src="data:image/png;base64,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"
        ></v-img>
      </v-avatar>
    </v-card>
    <v-card id="content4"></v-card>
    <!-- <v-card id="content3">Content3</v-card> -->
    <v-card elevation="6" id="footer">Footer</v-card>
  </v-layout>
</template>

<script>
export default {
  data: () => ({
    items: [
      { title: "Click Me" },
      { title: "Click Me" },
      { title: "Click Me" },
      { title: "Click Me 2" }
    ],
    offset: true
  })
};
</script>

<style>
:root {
  --main-radius: 5px;
  --main-padding: 5px;
}

body {
  font-family: "Inter", sans-serif;
}
#dpic {
  position: relative;
  bottom: -280px;
  border: white solid 5px;
}
#dpic2 {
  position: relative;
  bottom: -10px;
  right: 215px;
  border: white solid 3px;
  border-radius: 50%;
}
#container {
  display: grid;
  height: 200vh;

  grid-template-columns: 1.2fr 1fr 1fr 1fr;
  grid-template-rows: 0.2fr 1.5fr 1.2fr 0.8fr;
  grid-template-areas:
    "nav nav nav nav"
    "main main main main"
    "content4 content1 content2 content3"
    "footer footer footer footer";
  grid-gap: 1rem;
  font-weight: 800;

  font-size: 15px;
  color: #004d40;
  text-align: center;
}

nav {
  background: white;

  z-index: 2000;
  grid-area: nav;

  padding-top: var(--main-padding);
}
.dropdown-list {
  border-radius: 4px;
  background-color: white;
  position: relative;
  top: -25px;
  display: none;
  width: 6%;
  z-index: 1000000;
  box-shadow: 3px 3px rgb(0, 0, 0, 0.2);
  justify-content: center;
  align-content: center;

  transition: opacity 0.2s linear, visibility 0.2s linear;
}
.dropdown-list__item {
  padding: 1px;
  font-size: 18;
  justify-content: center;
  align-items: center;
  cursor: pointer;
}
.dropdown:hover .dropdown-list {
  display: block;
}

#main {
  background: white;
  grid-area: main;
  top: -40px;
  border-radius: 0px;
  padding-top: var(--main-padding);
}

#sidebar {
  background: white;
  grid-area: sidebar;
  border-radius: var(--main-radius);
  padding-top: var(--main-padding);
}

#content1 {
  background: white;
  grid-area: content1;
  width: 400px;
  position: relative;
  left: -9.5%;
  border-radius: var(--main-radius);
  padding-top: var(--main-padding);
  top: -35px;
}

#content2 {
  background: white;
  grid-area: content2;
  width: 520px;
  height: 100px;
  position: relative;
  right: 7.5%;
  border-radius: var(--main-radius);
  top: -35px;
}
#content4 {
  background: white;
  display: none;
  grid-area: content4;
  border-radius: var(--main-radius);
  padding-top: var(--main-padding);
}

#content3 {
  background: white;

  grid-area: content3;
  border-radius: var(--main-radius);
  padding-top: var(--main-padding);
}

#footer {
  background: #1de9b6;
  display: none;
  grid-area: footer;
  border-radius: var(--main-radius);
  padding-top: var(--main-padding);
}

a {
  text-align: center;
  display: block;
  font-family: inherit;
  text-decoration: none;
  font-weight: bold;
  margin: 1rem;
}
#main2 {
  position: relative;
  top: -25px;
  border-radius: var(--main-radius);
  min-height: 60vh;
  width: 65.5vw;
  left: 16.5%;
  background: linear-gradient(white, #f2f0f5, grey);
}
#main2 {
}
.line2 {
  height: 1px;
  background: rgb(162, 162, 162, 0.4);
  width: 63.5vw;
  left: 17.5%;
  z-index: 100000;
  top: 50px;
  position: relative;
}
.midnav2 {
  background: #dadada;
  width: 59.4vw;
  bottom: 0px;
  margin-bottom: 24px;
  padding: 3.5px;
  position: absolute;
  left: 17.5%;
  justify-content: left;
  align-items: left;
  display: flex;
}
.midnav {
  background: rgb(255, 255, 255);
  width: 59.4vw;
  bottom: -0;
  padding: 2.5px;
  position: absolute;
  left: 15.5%;
  justify-content: left;
  align-items: left;
  display: flex;
}
.navcon {
  color: gray;
  padding: 5px 20px;
  position: relative;
  text-align: left;
  display: flex;
  border-bottom: 3px solid blue;
  display: flex;
  transition: 0.4;
}
.navcon > a {
  color: inherit;
  text-decoration: none;
}
.navcon:hover {
  background-color: #f0f2f5;
  border-radius: 5px;
  height: inherit;

  padding: var(--main-padding);
  padding-top: var(--main-padding);
  color: blue;
}
.navcon {
  color: gray;
  padding: 10px 20px;
  position: relative;
  text-align: left;
  display: flex;
  border-bottom: 3px solid transparent;
  display: flex;
  transition: 0.4;
}
@media only screen and (max-width: 550px) {
  #container {
    height: 100vh;
    width: 100vw;
    grid-template-columns: 1fr;
    grid-template-rows: 0.01fr 1.2fr 0.5fr 1fr;
    grid-template-areas:
      "nav"
      "main"
      "content1"
      "content2"
      "footer";
  }
  #dpic {
    left: 26.5%;
    bottom: -50px;
    width: 120px;
    position: relative;
  }
  .dropdown-list {
    display: none;
  }
  #main {
    max-width: inherit;
  }
  #main2 {
    display: grid;
    position: absolute;

    left: 0px;
    right: 0px;
    z-index: 1;
    width: inherit;
    border-radius: 0px;
    min-height: 180px;
    background: linear-gradient(white, #f0f2f5, grey);
  }
  #content3 {
    margin: 8px;
    margin-top: 1px;
  }

  #content2 {
    margin: 15px;
    margin-top: 1px;
    width: inherit;
    left: 0px;
    right: 0px;
    padding: 0px;
  }
  #content1 {
    margin: 10px;
    height: 150px;
    left: 0px;
    right: 0px;
    margin-top: 0px;
  }
  .line {
    height: 1px;
    background: rgb(162, 162, 162, 0.4);
    width: inherit;

    z-index: 1;
    top: 200px;
    position: relative;
  }
  .line2 {
    display: none;
  }
  .midnav2 {
    background: #dadada;
    width: 59.4vw;
    bottom: 0px;
    margin-bottom: 24px;
    padding: 3.5px;
    position: absolute;
    left: 10.5%;
    justify-content: left;
    align-items: left;
    display: flex;
  }
  .midnav {
    background: rgb(255, 255, 255);
    width: inherit;
    bottom: -0;
    padding: 1.5px;
    position: absolute;
    left: 0;
    justify-content: left;
    align-items: left;
    display: flex;
  }
  .navcon {
    color: gray;
    padding: 10px 20px;
    position: relative;
    text-align: left;
    display: flex;
    border-bottom: 3px solid transparent;
    display: flex;
    transition: 0.4;
  }
  .navcon > a {
    color: inherit;
    text-decoration: none;
    font-size: 8px;
  }
  .navcon:hover {
    background-color: #f0f2f5;
    border-radius: 5px;
    color: blue;
  }
  .navcon {
    color: gray;
    padding: 5px 5px;
    position: relative;
    text-align: left;
    display: flex;
    border-bottom: 3px solid transparent;
    display: flex;
    transition: 0.4;
  }
}
</style>
