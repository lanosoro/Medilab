<template>
  <div style="position:relative; top:0px; bottom:20vh; height:250vh; width:100%;">
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
      <span style="line-height: 2.0em; font-family:inherit;">
        <li>
          {{ service }}
        </li>
      </span>
    </div>
    <div style="position:relative; top:1vh; right:0px; left:5px;">
      <p style="font-weight:600; font-size:18px; margin-left:5px;">We are committed to doing this by:</p>
     
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
        "Supply of quality food grade detergents to cater for all cleaning & hygiene needs.",
        "Preparation of a detailed cleaning manual for the factories to ensure a harmonized cleaning and hygiene system.",
        "Technical support to ensure good and consistent cleaning and hygiene results and to resolve quality challenges encountered from time to time.",
        "Analysis of utilities water( boilers, cooling towers, pasteurizers, ETP and process water treatment to confirm that the treatment regime are delivering the desired results.",
        "Quarterly trainings to ensure continuous improvement in the factories.",
        "Supply of high quality dosing and control equipment to ensure accurate and consistent dosing of the chemicals.",
        "Regular visit to the factory to monitor the cleaning and hygiene standards, and to identify any areas requiring urgent attention.",
        "Reports to the management indicating the levels of hygiene, cost trends against the budget, projects in progress and recommendations for improvements.",
        "Periodic audits for the entire factory to identify major improvement projects."
      ],
      commits: [
        "Investing the time to listen, understand and respond to customers’ unique cleaning and hygiene needs.",
        "Taking a personal interest to ensure the facilities they care for are consistently clean, safe and attractive.",
        "Pursuing innovation in every form likely to make the lives of our customers simpler and more profitable.",
        "Customer collaborating to exceed their expectations, every day, everywhere."
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
  height: 400px;
  display: "flex";
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
  .title{
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
  .title{
    font-size: 1px;
  }
}
</style>
