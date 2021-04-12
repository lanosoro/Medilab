<template>
  <v-layout
    class="hidden-sm-and-down fill-height "
    style="display:flex; flex-direction:column;"
    fluid
    ma-0
    pa-0
  >
    <!-- <header style="height:30px;">
      <bavbar />
    </header> -->

    <section
      id="landing"
      style="position:relative; top:-3px; height:100vh; background:rgba(255,255,255,0); width:100vw;"
    >
      <div class="sideimg">
        <img
          class="image"
          src="..\assets\school-chemistry-lab-equipment-500x500.jpg"
          alt=""
        />
        <img class="image" src="..\assets\Medical_supplies_small.jpg" alt="" />
        <img class="image" src="..\assets\tech.jpg" alt="" />
      </div>

      <div class="side"></div>
      <div class="container" id="glass">
        <h2>Welcome</h2>
        <h3>
          <span class="medilab"> Medilab & Allied Products K Ltd</span
          ><span style="color:black;">
            is located in Nairobi, Kenya, a Chemical & Research/Medical
            Distributor</span
          ><span style="color:black">
            We want to be a leading provider of products and services to the
            Medical, Water Treatment and scientific Sectors.
          </span>
        </h3>
        <a class="containera" href="products">Our Products</a>
      </div>
    </section>
    <section class="about" style="height:100vh;">
      <div class="card23" style="margin-bottom:100px: position:relative; bottom:20px;">
        <div class="content">
          <h1>About Us</h1>

          <h3 xtyle="font-weight:900"> <img src="" alt=""></h3>
          <p>
            Medilab & Allied Products K Ltd is a Kenyan company, which is
            committed to providing Medical and Research Reagents and
            Consumables, Water treatment chemicals, Cooling Tower/Boiler/Chiller
            chemicals and Condition Monitoring reagents/Sensors.
          </p>
          <a href="#">more</a>
        </div>
      </div>
      <div class="container3" style="top:100px;">
        <div class="card2">
          <div class="content">
            <h1>02</h1>

            <h3>Chemical Reagent</h3>
            <p>
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Fuga
              harum temporibus nisi culpa aspernatur reprehenderit a provident
              modi ab eius.
            </p>
            <a href="#">more</a>
          </div>
        </div>
        <div class="card2 " style="">
          <div class="content">
            

            <h3 style="  font-weight:900"> <img src="..\assets\F&B.png" alt="" height="50px"> Food & Beverages</h3>
            <p>
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Fuga
              harum temporibus nisi culpa aspernatur reprehenderit a provident
              modi ab eius.
            </p>
            <a href="#">more</a>
          </div>
        </div>
        <div class="card2">
          <div class="content">
            <h1> </h1>
            <h3 style="display:block; font-weight:900"> <img src="..\assets\personalcareicon.png" alt="" height="50px">personal hyiene </h3>
            <p>
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Fuga
              harum temporibus nisi culpa aspernatur reprehenderit a provident
              modi ab eius.
            </p>
            <a href="#">more</a>
          </div>
        </div>
        <div class="card2">
          <div class="content">
            <h3>water treatment reagents</h3>
            <p>
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Fuga
              harum temporibus nisi culpa aspernatur reprehenderit a provident
              modi ab eius.
            </p>
            <a href="#">more</a>
          </div>
        </div>
      </div>
    </section>
    <section class="products" id="products">
      <div class="container2">
        <div class="card">
          <div class="cotent">
            
            <h1>01</h1>
            <img
              height="120px"
              width="200px"
              src="..\assets\380-3808023_medical-supplies-medical-supplies-transparent.png"
              alt=""
            />
            <h3>Medical supplies</h3>
            <p>
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Fuga
              harum temporibus nisi culpa aspernatur reprehenderit a provident
              modi ab eius.
            </p>
            <a href="#">more</a>
          </div>
        </div>
        <div class="card">
          <div class="cotent">
            <h1>02</h1>
            <img
              height="120px"
              src="..\assets\158-1584784_how-chemical-cleaning-supplies-can-help-you-boost.png"
              alt=""
            />
            <h3>Chemical Reagent</h3>
            <p>
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Fuga
              harum temporibus nisi culpa aspernatur reprehenderit a provident
              modi ab eius.
            </p>
            <a href="#">more</a>
          </div>
        </div>
        <div class="card">
          <div class="cotent">
            <h1>03</h1>
            <!-- <img
              height="120px"
              src="..\assets\Important-Processes-for-Food-Processing-and-Packaging.jpg"
              alt=""
            /> -->
            <h3>Processing factory</h3>
            <p>
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Fuga
              harum temporibus nisi culpa aspernatur reprehenderit a provident
              modi ab eius.
            </p>
            <a href="#">more</a>
          </div>
        </div>
      </div>
    </section>
    <section class="products">
      <div class="container">
        <div class="card">
          <div
            class="cotent  col-lg-12 col-lg-2 col-lg-3 col-lg-4 col-lg-5 col-lg-6 col-lg-7 col-lg-8 col-lg-9 col-lg-auto col-md col-md-1 col-md-10 col-md-11 col-md-12 col-md-2 col-md-3 col-md-4 col-md-5 col-md-6 col-md-7 col-md-8 col-md-9"
          >
            <div class="contact-form">
              <span class="circle-one"> </span>
              <span class="circle-two"></span>
              <form>
                <h3 class="title-3">Contact us</h3>
                <div class="input-container">
                  <input
                    type="text"
                    name="name"
                    class="input"
                    placeholder="Username"
                  />
                  <label for="">Username</label>
                </div>
                <div class="input-container">
                  <input
                    type="email"
                    name="email"
                    class="input"
                    placeholder="Email"
                  />
                  <label for="">Email</label>
                </div>
                <div class="input-container">
                  <input
                    type="tel"
                    name="phone"
                    class="input"
                    placeholder="phone"
                  />
                  <label for="">Phone</label>
                </div>
                <div class="input-container textarea">
                  <textarea name="" id="" rows="4" placeholder="message">
                  </textarea>
                  <label for="">message</label>
                </div>
                <input type="submit" value="send" class="btn" />
              </form>
            </div>
          </div>
        </div>
      </div>
    </section>
  </v-layout>
</template>
<script>
import anime from "animejs/lib/anime.es.js";

export default {
  data() {
    {
      var textWrapper = document.querySelector(".medilab .letters");
      textWrapper.innerHTML = textWrapper.textContent.replace(
        /\S/g,
        "<span class='medilab'>$&</span>"
      );

      anime
        .timeline({ loop: true })
        .add({
          targets: ".medilab",
          rotateY: [-90, 0],
          duration: 1300,
          delay: (el, i) => 45 * i
        })
        .add({
          targets: ".medilab",
          opacity: 0,
          duration: 1000,
          easing: "easeOutExpo",
          delay: 1000
        });
    }
  }
};
</script>

<style scoped>
/* about section */
.about {
     position: relative;
    display: flex;
    padding: 40px;
    flex-direction: row;
    justify-content: center;
    max-width: 100vw;
    flex-wrap: wrap;
    z-index: 100;
    align-items: center;
}

.container3 {
  margin: 0;
  display: flex;
  align-items: center;
  justify-content: center;
  background: rgb(255, 255, 255);
}

/* end */
#landing {
  font-family: noto sans;
  padding: 14em 14em 14em 20em;
  margin: 0;
  position: relative;
  top: -100px;
}
.sideimg {
  z-index: -1;
  position: absolute;
  height: 100vh;
  width: 100vw;
  top: 0;
  left: 0;
  background: rgba(0, 187, 255, 0.597);
}
.containera {
  position: relative;
  display: inline-block;
  padding: 8px 25px;
  margin-top: 15px;
  background: rgba(0, 0, 0, 0.024);
  font-weight: 700;
  font-size: 1.15rem;
  box-shadow: 0 5px 5px rgb(0 0 0 / 43%);
  border-radius: 10px;
  text-decoration: none;
  color: white;
}
.image {
  height: 100vh;
  width: 503px;
  opacity: 0.3;
  z-index: -1000000;
  margin-left: -5px;
}
.side {
  top: 200px;
  left: 200px;
  position: absolute;
  width: 400px;
  height: 400px;
  background: rgb(8, 195, 220);
  border-radius: 50%;
  display: none;
  z-index: -1;
}
.medilab {
  font-size: 3rem;
  font-weight: 900;
  color: white;
}
.container {
  display: inline-block;
  background: rgba(243, 243, 243, 0);
 
  padding: 3em;
 align-content: center;
 justify-items: center;
  border-radius: 3em;
  top: -15px;
 
  position: relative;
  z-index: 1;
  -webkit-backdrop-filter: blur(4px);
  backdrop-filter: blur(4px);
  border: solid 2px transparent;
  background-clip: padding-box;
}

.conatainer h3 {
  margin: 0;
  font-size: 2rem;
  color: blue;
  flex-wrap: wrap;
  width: 50vw;
}

h2 {
  font-size: 2.6em;
  font-weight: 1000;
}
li {
  float: left;
  line-height: 30px;
  padding: 0px 10px;
  word-wrap: normal;
  list-style-type: none;
}
.main-tag {
  position: relative;
  top: 50%;
  left: 15%;
}
.main-tag h2 {
  color: white;
  font-family: noto sans;
  position: relative;
  font-size: 45px;
  top: 50vh;
}
/* section 2 */
.products {
  min-height: 100vh;
  margin: 0;
  display: flex;

  align-items: center;
  justify-content: center;
  background: rgb(255, 255, 255);
}

.container2 {
    position: relative;
    display: flex;
    flex-direction: row;
    justify-content: center;
    max-width: 100vw;
    flex-wrap: wrap;
    z-index: 100;
    top: 140px;
    align-items: center;
}
.container2 .card {
  position: relative;
  font-family: noto sans;
  font-size: 14px;
  width: 280px;
  top: 100px;
  height: 345px;
  padding: 19px;
  margin: 50px;
  margin-bottom: 90px;
  box-shadow: 20px 20px 40px rgba(0, 0, 0, 0.426);
  border-radius: 15px;
  background: rgba(0, 187, 255, 0.145);
  border-top: 1px solid rgba(252, 252, 252, 0.4);
  border-left: 1px solid rgba(252, 252, 252, 0.4);
  justify-content: center;
  align-items: center;
  backdrop-filter: blur(5px);
}
.container2 .card .cotent {
  padding: 10px;
  text-align: left;
  transition: 0.5s;
  transform: translateY(10px);
  opacity: 0.5;
}
.container2 .card:hover .cotent {
  transform: translateY(0px);
  opacity: 1;
}
.container2 .card .cotent h1 {
  position: absolute;
  top: -10px;
  right: 30px;
  font-size: 3em;
  color: rgba(0, 0, 0, 0.426);
  pointer-events: none;
}
/* contact section */
.col-lg-12,
.col-lg-2,
.col-lg-3,
.col-lg-4,
.col-lg-5,
.col-lg-6,
.col-lg-7,
.col-lg-8,
.col-lg-9,
.col-lg-auto,
.col-md,
.col-md-1,
.col-md-10,
.col-md-11,
.col-md-12,
.col-md-2,
.col-md-3,
.col-md-4,
.col-md-5,
.col-md-6,
.col-md-7,
.col-md-8,
.col-md-9 {
  position: relative;
  width: 100%;
  min-height: 1px;
  padding-right: 0;
  padding-left: 0;
}
.products {
  min-height: 100vh;
  margin: 0;
  display: flex;
  align-items: center;
  justify-content: center;
  background: rgb(255, 255, 255);
}
.products::before {
  content: "";
  position: absolute;
  display:none;
  top: 40vh;
  left: 0;
  width: 100%;
  height: 100%;
  background: linear-gradient(rgba(0, 187, 255, 0.597), white);
  clip-path: circle(30% at right 50%);
}
.products::after {
  content: "";
  position: absolute;
  top: 40px;
  display: none;
  left: 0;
  z-index: 0;
  width: 100%;
  height: 100%;
  background: linear-gradient(rgba(0, 187, 255, 0.056), white);
  clip-path: circle(20% at 10% 40%);
}
.container {
  position: relative;
  display: flex;
  justify-content: center;
  max-width: 1200px;
  flex-wrap: wrap;
  z-index: 10000;
  overflow: hidden;
}
.container .card {
      position: relative;
    font-family: noto sans;
    font-size: 14px;
    width: 302px;
    top: 100px;
    height: 373px;
    padding: 11px;
    margin: 7px;
    margin-bottom: 90px;
    box-shadow: 20px 20px 40px rgb(0 0 0 / 43%);
    border-radius: 15px;
    background: rgba(0, 187, 255, 0.145);
    border-top: 1px solid rgba(252, 252, 252, 0.4);
    border-left: 1px solid rgba(252, 252, 252, 0.4);
    justify-content: center;
    align-items: center;
    -webkit-backdrop-filter: blur(5px);
    backdrop-filter: blur(5px);
}
.container .card .cotent {
  padding: 10px;
  text-align: left;
  transition: 0.5s;
  transform: translateY(10px);
  opacity: 1;
}
.container .card:hover .cotent {
  transform: translateY(0px);
  opacity: 1;
}

.container .card .cotent h1 {
  position: absolute;
  top: -10px;
  right: 30px;
  font-size: 3em;
  color: rgba(0, 0, 0, 0.426);
  pointer-events: none;
}

.container .card .cotent a {
  position: relative;
  display: inline-block;
  padding: 8px 25px;
  margin-top: 15px;
  background: rgba(1, 217, 255, 0.324);
  font-weight: 500;
  box-shadow: 0 5px 5px rgba(0, 0, 0, 0.426);
  border-radius: 10px;
  text-decoration: none;
}
#lastcard {
  margin-bottom: 230px;
}
.contact-container {
  position: relative;
  width: 100%;
  min-height: 100vh;
  padding: 2rem;
  background: #fafafa;
  overflow: hidden;
  display: flex;
  align-items: center;
  justify-content: center;
}
.form {
  width: 100%;
  max-width: 820px;
  height: 100%;
  background-color: #fff;
  border-radius: 10px;
  z-index: 10000;
  box-shadow: 0 0 20px 1px rgba(0, 16, 242, 0.761);
  grid-template-columns: repeat(2, 1fr);
  display: grid;
}
.contact-form {
  background-color: transparent;
  position: relative;
  border-top-right-radius: 10px;
  border-bottom-right-radius: 10px;
}
.circle-one {
  width: 100px;
  height: 100px;
  border-radius: 50%;
  position: absolute;
}
form {
  padding: 2.3rem 2.2rem;
  z-index: 10;
  overflow: hidden;
  position: relative;
}
.title-3 {
  color: white;
  font-weight: 500;
  font-size: 1.5rem;
  line-height: 1;
  margin-bottom: 0.7rem;
}
label {
  display: none;
}
input {
  width: 100%;
  margin-bottom: 30px;
  outline: none;
  border: 2px solid #fafafa;
  background: none;
  padding: 0.6rem 1.2rem;
  position: relative;
  left: -10px;
  color: #fff;
  font-weight: 500;
  font-size: 0.95rem;
  letter-spacing: 0.5px;
  border-radius: 25px;
  transition: 0.3s;
  z-index: 1000000;
}

textarea.input {
  padding: 0.8rem 1.2rem;
  min-height: 150px;
  border-radius: 22px;
  resize: none;
  overflow-y: auto;
  border: none;
  outline: 1px solid white;
  background: #fafafa;
}
.btn {
  padding: 0.6rem 1.3rem;
  background-color: #fff;
  border: 2px solid #fafafa;
  font-size: 0.95rem;
  color: #1abc9c;
  line-height: 1;
  border-radius: 25px;
  outline: none;
  cursor: pointer;
  transition: 0.3s;
  margin: 0;
}

.btn:hover {
  background-color: transparent;
  color: #fff;
}
/* .input-container label {
  position: absolute;
  top: 50%;
  left: 15px;
 
  padding: 0 0.4rem;
  color: #fafafa;
  font-size: 0.9rem;
  font-weight: 400;
  pointer-events: none;
  z-index: 1000;
  transition: 0.5s;
} */

.input-container.textarea label {
}
.input-container span {
  position: absolute;
  top: 0;
  left: 25px;
  transform: translateY(-50%);
  font-size: 0.8rem;
  padding: 0 0.4rem;
  color: transparent;
  pointer-events: none;
  z-index: 500;
}

.input-container span:before,
.input-container span:after {
  content: "";
  position: absolute;
  width: 10%;
  opacity: 1;
  transition: 0.3s;
  height: 5px;
  background-color: #1abc9c;
  top: 50%;
  transform: translateY(-50%);
}

.input-container span:before {
  left: 50%;
}

.input-container span:after {
  right: 50%;
}

@media (max-width: 500px) {
  .cotent {
    width: 100%;
    padding: 30px;
  }
  #landing{
      font-family: noto sans;
    padding: 2em 2em 2em 4em;
    margin: 0;
    position: relative;
    top: -100px;
}
  .container .card {
    position: relative;
    font-family: noto sans;
    font-size: 14px;
    width: 100%;
    top: 10px;
    height: 100%;
    padding: 1px;
    margin: 3px 0;
    margin-bottom: 9px;
    box-shadow: 20px 20px 20px rgb(0 0 0 / 43%);
    border-radius: 15px;
    background: rgba(0, 187, 255, 0.166);
    border-top: 1px solid rgba(252, 252, 252, 0.4);
    border-left: 1px solid rgba(252, 252, 252, 0.4);
    justify-content: center;
    align-items: center;
    -webkit-backdrop-filter: blur(5px);
    backdrop-filter: blur(5px);
  }

.container2 .card .cotent a {
  position: relative;
  display: inline-block;
  padding: 8px 25px;
  margin-top: 15px;
  background: rgba(1, 217, 255, 0.324);
  font-weight: 500;
  box-shadow: 0 5px 5px rgba(0, 0, 0, 0.426);
  border-radius: 10px;
  text-decoration: none;
}
#lastcard {
  margin-bottom: 230px;
}
}
/* end */
@media screen and (max-width: 991px) {
  #landing{
    font-family: noto sans;
    padding: 7em 7em 7em 10em;
    margin: 0;
    position: relative;
    top: -100px;
}
  .image {
    height: 100vh;
    width: 503px;
    display: none;
    opacity: 0.3;
    z-index: -1000000;
    margin-left: -5px;
  }
    .container .card {
    position: relative;
    font-family: noto sans;
    font-size: 14px;
    width: 100%;
    top: 10px;
    height: 100%;
    padding: 1px;
    margin: 3px 0;
    margin-bottom: 9px;
    box-shadow: 20px 20px 20px rgb(0 0 0 / 43%);
    border-radius: 15px;
    background: rgba(0, 187, 255, 0.166);
    border-top: 1px solid rgba(252, 252, 252, 0.4);
    border-left: 1px solid rgba(252, 252, 252, 0.4);
    justify-content: center;
    align-items: center;
    -webkit-backdrop-filter: blur(5px);
    backdrop-filter: blur(5px);
  }
  
  .container {
  display: inline-block;
    background: rgba(243, 243, 243, 0.145);
    width: 60vw;
    padding: 1em;
    border-radius: 3em;
    top: -0px;
    position: relative;
    z-index: 1;
    -webkit-backdrop-filter: blur(4px);
    backdrop-filter: blur(4px);
    border: solid 2px transparent;
    background-clip: padding-box;
    box-shadow: 10px 10px 10px rgb(255 255 255 / 30%);}
  .conatainer h3 {
    margin: 0;
    font-size: 1.5rem;
    color: blue;
    flex-wrap: wrap;
    width: 50vw;
  }

  h2 {
    font-size: 2.6em;
    font-weight: 1000;
  }
}
@media screen and (max-width: 600px) {
.about .container3 .content p{
    margin-top: 0;
    margin-bottom: 1rem;
    align-items: center;
    text-align: center;
    line-height: 1.5rem;

}
#landing{
      font-family: noto sans;
    padding: 4em 4em 4em 7em;
    margin: 0;
    position: relative;
    top: -100px;
}
  .image {
    height: 100vh;
    width: 503px;
    opacity: 0.3;
    z-index: -1000000;
    display: none;
    margin-left: -5px;
  }
  .container {
    display: inline-block;
    background: rgba(243, 243, 243, 0.145);
    width: 80vw;
    left: -0vw;
    padding: 1em;
    border-radius: 3em;
    top: -0px;
    position: relative;
    z-index: 1;
    -webkit-backdrop-filter: blur(4px);
    backdrop-filter: blur(4px);
    border: solid 2px transparent;
    background-clip: padding-box;
    box-shadow: 10px 10px 10px rgb(255 255 255 / 30%);
  }
  .conatainer h3 {
    margin: 0;
    font-size: 1.5rem;
    color: blue;
    flex-wrap: wrap;
    width: 50vw;
  }

  h2 {
    font-size: 2.6em;
    font-weight: 1000;
  }
  .container3[data-v-19c9d02c] {
    margin: 0;
    display: flex;
    align-items: center;
    justify-content: center;
    background: transparent;
    width: 100%;
    top: 100px;
    position: relative;
    flex-direction: column;
    height: 100%;
}



.container-form{
    display: inline-block;
    background: rgba(243, 243, 243, 0.145);
    width: 86vw;
    left: 1vw;
    padding: 1em;
    border-radius: 2em;
    top: 20px;
    position: relative;
    z-index: 5;
    -webkit-backdrop-filter: blur(4px);
    backdrop-filter: blur(4px);
    border: solid 2px transparent;
    background-clip: padding-box;
    box-shadow: 10px 10px 10px rgb(255 255 255 / 25%);
}

}
</style>
