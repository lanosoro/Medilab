<template>
  <section class="project-area">
    <div class="container">
      <div class="project-title pt-4">
        <h1 class="text-uppercase title-h1">
          Products Range
        </h1>
      </div>
      <div class="button-group">
        <button type="reset" class="active">All</button>
        <button type="reset" data-filter="water">Water Treatement</button>
        <button type="reset" data-filter="medical">Medical</button>
        <button type="reset">Scientific</button>
      </div>
      <div class="row grid">
        <div class="col-lg-4 col-md-6 col-sm-12 element-item water">
          <div class="our-products">
            <div class="image">
              <img src="@/assets/watertreatmenticon.png" alt="">
            </div>
            <div class="title py-4">
              <h4 style="font-weight:700" class="text-uppercase">
                water treatment
              </h4>
              <span class="text-secondary">
                water treatment chemicals Solutions
              </span>
            </div>
            
          </div>
          
        </div>
        <div class="col-lg-4 col-md-6 col-sm-12 element-item latest">
          <div class="our-products">
            <div class="image">
              <img src="@/assets/kitchenhygieneicon.png" alt="">
            </div>
            <div class="title py-4">
              <h4 style="font-weight:700" class="text-uppercase">
                water treatment
              </h4>
              <span class="text-secondary">
                water treatment chemicals Solutions
              </span>
            </div>
            
          </div>
          
        </div>
        <div class="col-lg-4 col-md-6 col-sm-12 element-item medical">
          <div class="our-products">
            <div class="image">
              <img src="@/assets/personalcareicon.png" alt="">
            </div>
            <div class="title py-4">
              <h4 style="font-weight:700" class="text-uppercase">
                personal hygiene
              </h4>
              <span class="text-secondary">
                water treatment chemicals Solutions
              </span>
            </div>
            
          </div>
          
        </div>
        <div class="col-lg-4 col-md-6 col-sm-12 element-item latest">
          <div class="our-products">
            <div class="image">
              <img src="@/assets/workshopicon.png" alt="">
            </div>
            <div class="title py-4">
              <h4 style="font-weight:700" class="text-uppercase">
                Workshop
              </h4>
              <span class="text-secondary">
                water treatment chemicals Solutions
              </span>
            </div>
            
          </div>
          
        </div>
      </div>
    </div>
  </section>
</template>

<script>

export default {

}
</script>

<style scoped>
.container{
  display: block;
}
.button-group{
  justify-content: space-around;
  justify-items: stretch;
}
button{
  padding: 15px;
  background: transparent;
  font: 600 19px/130px;
  font-weight: 700;
  left: 5px;
  color: black;
  border: none;
  text-transform: uppercase;
  position: relative;
}
button + button{
  padding-left: 3rem;
}
button:focus,button:active,button:hover,.btn:active,.btn.active{
  outline: 0px !important;
  box-shadow: rgba(0, 0, 0, 0.3);
}
.project-area{
  padding: 4rem 0;
}
</style>