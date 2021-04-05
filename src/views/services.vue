<template>
  <div
    style="position:relative; top:0px; bottom:20vh; height:250vh; width:100%;"
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
          <div class="services_page" elevation="5">
            <v-card-title
              class="title"
              style="position:relative; left:0px; top:20px;  font-size: 8vh;"
              >Our Services</v-card-title
            >
          </div>
        </v-carousel-item>
      </v-carousel>
    </div>
    <div
      class="services col-md-12  row container-fluid"
      v-for="service in services"
      :key="service"
    >
      <span style="line-height: 3.0em; font-family:inherit;">
        <li>
          {{ service }}
        </li>
      </span>
    </div>

    <div class="commitment" v-for="commit in commits" :key="commit">
      <ul style="">
        <li>
          {{ commit }}
        </li>
      </ul>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      slides: ["servicesbanner.jpg"],
      services: [
        "edilab & Allied Products K Ltd is a Kenyan company, which is committed to providing Medical and Research Reagents and Consumables, Water treatment chemicals, Cooling Tower/Boiler/Chiller chemicals and Condition Monitoring reagents/Sensors."
      ],
      commits: [
        "Our Customers:",
        "Power Plants",
        "Research Institutions",
        "Hospitals",
        "Food Processors",
        "Across East and West"
      ],

      products_lable: [
        "KITCHEN HYGIENE",
        "HOUSE KEEPING",
        "FOOD & BEVERAGE  ",
        "CONVEYER SYSTEM",
        "PERSONAL CARE",
        "WORKSHOP",
        "LAUNDRY",
        "WATER TREATMENT",
        "SPECIALTIES"
      ]
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
  height: 100vh;
  display: "flex";
  justify-content: space-between;
  align-content: center;
  font-size: 19px;
}
.services {
  position: relative;
  top: 10vh;
  right: 0px;
  left: 50px;
}
.commitment {
  position: relative;
  top: 15vh;
  right: 0px;
  left: 10px;
  flex: wrap;
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
@media only screen and (max-width: 768px) {
  .services {
    position: relative;
    top: 0vh;
    left: 10px;
  }

  .services_page {
    position: absolute;
    margin-bottom: -290px;
    display: inline-block;
    font-size: 18px;
    left: 250px;
    right: 0px;
    width: 100%;
    height: 260px;
    z-index: 99;

    background-color: rgba(0, 116, 165, 0.6);
  }
  .title {
    font-size: 100px;
  }
}
@media only screen and (max-width: 345px) {
  .services {
    position: relative;
    top: 0vh;
    left: 10px;
  }

  .services_page {
    position: absolute;
    margin-bottom: -290px;
    display: inline-block;
    font-size: 13px;
    left: 250px;
    right: 0px;
    width: 100%;
    height: 260px;
    z-index: 99;

    background-color: rgba(0, 116, 165, 0.6);
  }
  .title {
    font-size: 1px;
  }
}
</style>
