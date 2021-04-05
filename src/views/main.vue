<template>
  <section>
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
        <div class="header col-lg-4 col-md-6 col-sm-12">
             <div class="container">
       
          <div class="row">
              <div class="col-lg-6 col-md-12 site-title">
                  <h3 class="title-text">
                      Welcome!
                  </h3>
                  <h1 class="title text-uppercase" style="font-size:45px;">
                      Medilab Allied
                  </h1>
                  <p class="para">
                    Medilab & Allied 
                    Products K Ltd is 
                    located in Nairobi, 
                    Kenya, a Chemical & 
                    Research/Medical 
                    Distributor
                  </p>
                  <p class="para">
                    We want to be a 
                    leading provider of 
                    products and 
                    services to the 
                    Medical, Water 
                    Treatment and 
                    scientific Sectors.
                  </p>
                  <div class="site-buttons">
                      <div class="d-flex flex-row flex-wrap">
                          <a href="/products"><button type="button" style="background: blue; color:white; padding:20px; border-radius:10px;" class="btn button primary-button mr-4 text-uppercase">Products</button></a>
                      </div>
                  </div>
              </div>
              <div class="col-lg-6 col-md-12">
                  
              </div>
          </div>
      </div>
        </div>
      </v-carousel-item>
    </v-carousel>
     
  </section>
</template>

<script>
export default {
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
}
</script>

<style scoped>
section{
    background: white;
    background-size: 100%;
}
.container h3{
    padding-top: 15%;
    font-weight: 500;
}
.container h3::after{
    content:"";
    height: 2px;
    width: 14vw;
    background: black;
    display: inline-block;
    margin-left: 5%;
    transform: translateY(-10px);

}
.header{
    position: absolute;
    background: rgba(0,0,0,0.4);
    color: blanchedalmond;
    overflow: clip;
    left: 0px;
    top: 20%;
    width: 40vw;
}
.para{
    color: white;
    width: 600px;

}
@media screen and (min-width:350px) {
    .header{
            position: absolute;
    background: rgba(0,0,0,0.4);
    color: blanchedalmond;
    overflow: clip;
    left: 0px;
    top: 20%;
    width: 100%;
    }
}
</style>