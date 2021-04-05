<template>
  <section class="main">
    <v-container class="fluid">
      <v-row class="row">
        <v-col>
          <div class="main-image col-lg-14 col-md-14">
          
            
          <div class="col-lg-14 col-md-14">
             <img class="image" height="400px" width="100%" src="@/assets/londro.jpg" alt="fire extinguisher">
          </div>
              <div class="col-lg-12 col-md-14 main-title">
                
                <h2 class="text-uppercase pt-4">
                 About Medilab Allied
                </h2>
                <div class="paragraph py-4 w-75">
                  <p class="para" style="font-size:18px; color:black;font-weight:600; ">
                    Medilab & Allied Products K Ltd is a Kenyan company,<br> which is committed to providing Medical and Research Reagents and Consumables,<br>
                    Water treatment chemicals, Cooling Tower/Boiler/Chiller chemicals and Condition Monitoring reagents/Sensors.
                  </p>
               
                  <button style="background: blue; color:white; padding:20px; border-radius:10px;" type="button" class="btn primary-button text-uppercase">
                    <a style="text-decoration:none; color:white; padding:30px" href="#">Learn More</a>
                  </button>

                </div>
              </div>
          </div>
        </v-col>

      </v-row>
    </v-container>
  </section>
</template>

<script>
export default {

}
</script>

<style scoped>
.main{
  padding: 3rem 2rem;
}
.main .main-title >h2{
  font: normal bold 49px/60px ;
  display: block;
  font-weight: 900;
  letter-spacing: 15px;
}
.row{
  display: flex;
  flex-direction: row;
  
}

.main-image{
   display: flex;
  flex-direction: row;
  justify-content: space-between;
}

.image{
  position: relative;
  left: -100px;
}
@media  (max-width: 991px) {
  .main-image{
    display: flex;
    flex-direction: column;
    overflow: auto;
  }
}
@media  (min-width: 301px) {
  .main-image{
    display: flex;
    flex-direction: column-reverse;
    overflow: auto;
    width: 100%;
  }
  p{
    width: 85vw;
    
    overflow: hidden;
  }


}
</style>