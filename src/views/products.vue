<template>
  <div
    id="container"
    style="position:relative; top:0px; bottom:20vh; width:100%;"
  >
    <div class="Main">
      <v-carousel
        hide-delimiters
        :controls="false"
        :indicators="false"
        :interval="3000"
        direction="up"
        :show-arrows="false"
        style="height:400px top:100px;"
      >
        <v-carousel-item
          v-for="(item, i) in slides"
          :key="i"
          :src="require('../assets/' + item)"
        >
          <v-card class="services_page" elevation="5">
            <v-card-title
              class="overlay"
              style="position:relative; left:0px; top:20px;  font-size: 8vh;"
              >Products</v-card-title
            >
          </v-card>
        </v-carousel-item>
      </v-carousel>
    </div>
    <products />
  </div>
</template>
<script>
import products from "../components/products.vue";
export default {
  components: { products },
  data() {
    return {
      slides: ["products.jpg"]
    };
  }
};
</script>
<style scoped>
.products_card {
  margin-left: 25px;
  margin-top: 10px;
  width: 15vw;
  height: 250px;
  background-color: #ccccff;
  display: flex;
}
.container {
  height: 300px;
  display: "flex";
  min-height: 100vh;
}
.services {
  position: relative;
  top: 10vh;
  right: 0px;
  left: 50px;
}
.main {
  height: 100%;
}
.commitment {
  position: relative;
  top: 15vh;
  right: 0px;
  left: 50px;
}
#products {
  padding: 100px;
  position: relative;
  bottom: 40px;
  left: 8%;
}
.services_page {
  position: absolute;
  top: 50%;
  left: 50%;
  height: 100px;
  transform: translate(-50%, -50%);
  z-index: 99;
  background-color: rgba(0, 116, 165, 0.6);
  border-radius: 10px;
}
.productcontainer {
  display: block;
}
.productcategory {
  display: flex;
  flex-direction: column;
  width: 18%;
  background-color: #f2f2f2;
  border-radius: 10px;
  margin: 1%;
  text-align: center;
  flex-direction: column;
  float: left;
  padding: 20px;
  justify-content: center;
  align-items: center;
  padding: 50px 80px;
}
@media only screen and (max-width: 400px) {
  #container {
    height: 100%;
    overflow: auto;
  }
  .services {
    position: relative;
    top: 0vh;
    left: 10px;
  }
  #products {
    height: 150vh;
    display: block;
    position: relative;
    right: 100pxsss;
  }
  .productcontainer {
    align-content: center;
  }
  .productcategory {
    display: flex;
    flex-direction: column;
    width: 45vw;
    position: relative;
    left: 28%;
    background-color: #f2f2f2;
    border-radius: 10px;
    margin: 1%;
    text-align: center;

    flex-direction: column;

    justify-content: center;
    align-items: center;
    padding: 50px 80px;
  }

  .services_page {
    position: absolute;
    bottom: -290px;
    display: inline-block;
    left: 200px;
    right: 0px;
    width: 100%;
    height: 260px;
    z-index: 99;

    background-color: rgba(0, 116, 165, 0.6);
  }
}
@media only screen and (max-width: 758px) {
  #container {
    height: 100%;
    overflow: auto;
  }
  .services {
    position: relative;
    top: 0vh;
    left: 10px;
  }
  #products {
    height: 100%;
    display: block;
  }
  .productcontainer {
    align-content: center;
  }
  .productcategory {
    display: flex;
    flex-direction: column;
    width: 45vw;
    position: relative;
    left: 28%;
    background-color: #f2f2f2;
    border-radius: 10px;
    margin: 1%;
    text-align: center;

    flex-direction: column;

    justify-content: center;
    align-items: center;
    padding: 50px 80px;
  }

  .services_page {
    position: absolute;
    bottom: -290px;
    display: inline-block;
    left: 250px;
    right: 0px;
    width: 100%;
    height: 260px;
    z-index: 99;

    background-color: rgba(0, 116, 165, 0.6);
  }
}
</style>
