<template>
  <v-layout id="container">
    <div class="over"></div>
    <v-carousel
      id="display"
      cycle
      height="650"
      width="100vw"
      hide-delimiter-background
      show-arrows-on-hover
      hide-delimiters
      hide-arrows
      :show-arrows="false"
    >
      <v-carousel-item v-for="(slide, i) in slides" :key="i" :src="slide.src">
        <div class="header">
          <h1 style="margin-left:5vw; margin-top:8%;">{{ slide.info }}</h1>
          <p style="margin-left:5vw; margin-top:30px;">{{ slide.body }}</p>
        </div>
      </v-carousel-item>
    </v-carousel>
    <bodycom/>
  </v-layout>
</template>

<script>
import bodycom from '../components/bodycom.vue';
export default {
  components: {bodycom},
  data() {
    return {
      colors: [
        "http://www.odexchemicals.com/wp-content/uploads/2020/09/contactusbanner.jpg",
        "warning",
        "pink darken-2",
        "red lighten-1",
        "deep-purple accent-4"
      ],
      justify: ["start", "center", "end", "space-around", "space-between"],
      slides: [
        {
          src:
            "http://www.odexchemicals.com/wp-content/uploads/2020/09/homeslider01.jpg",
          info: "25 years of expertise",
          body: "we manufacture specialized deterents and sanitation products"
        },
        {
          src:
            "http://www.odexchemicals.com/wp-content/uploads/2020/09/HouseKeeping-Range.jpg",
          info: "We are the hygiene solution",
          body: "we have a wide range of housekeeping Solutions"
        },
        {
          src:
            "http://www.odexchemicals.com/wp-content/uploads/2020/09/Conveyer-Systems-Slider.jpg",
          info: "Wide Range of products",
          body: "Check out our conveyor Lubes"
        }
      ]
    };
  }
};
</script>

<style scoped>
.home-card {
  background: #333;

  width: 100%;
  color: white;
}

#container {
  display: block;
}
.over {
  position: absolute;
  bottom: 30%;
  left: 0;

  z-index: 99;
  width: 60%;
  background-color: rgba(0, 116, 165, 0.6);
  border-top-right-radius: 10px;
  border-bottom-right-radius: 10px;
}
#display {
  position: relative;
  left: 0;
}
.header {
  position: absolute;
  bottom: 30%;
  display: block;
  left: 0;
  width: 903px;
  height: 260px;
  z-index: 99;
  width: 60%;
  background-color: rgba(0, 116, 165, 0.6);
  border-top-right-radius: 10px;
  border-bottom-right-radius: 10px;
}
.card-title {
  display: flex;
  align-items: center;
  background: #222;
  border-radius: 8px;
}
.subtitle {
  display: grid;
}
.avatar {
  widows: 50px;
  border: 1px solid rgba(255, 255, 255, 0.4);
  border-radius: 50%;
  margin: 5px 30px;
}
.subtitle > p {
  margin-bottom: 0;
  color: blue;
}
.card-content {
  line-height: 1.5;
  margin: 30px auto;
}
table {
  border-spacing: 0px;
  margin: 50px auto;
}
tr th,
tr td {
  border: 1px solid white;
  border-top: none;
  padding: 10p;
  text-align: none;
}
table :first-of-type {
  border-left: none;
}
table :nth-of-type(2) {
  border-right: none;
}
#footer {
  position: absolute;
  bottom: 0;
}
@media screen and (max-width: 1096px) {
  #display {
    height: 400px;
  }
  .header {
    position: absolute;
    bottom: 0%;
    left: 0px;
    right: 0px;
    max-width: 1096px;
    height: 260px;
    z-index: 99;
    width: 60%;
    background-color: rgba(0, 116, 165, 0.6);
  
  }
}
</style>
