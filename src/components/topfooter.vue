<template>
  <v-layout>
    <div class="tfcontent">
      <v-flex column>
        <div class="tfcontent-item" id="contacts">
          <span id="contactus">Contact Us</span>
          <div class="contacts">
            <p style="color:#999;">
              MEDILAB AND ALLIED PRODUCTS (K) LTD, <br />
              GENERAL WARUINGE ROAD,<br />
              OLD RACE COURSE, STAREHE COURT 7638 (2),<br />
              P.O BOX 14705-00400,<br />
              NAIROBI, KENYA <br />
              TEL: +254 721 811 499, +254 734 768 110, +254 020 4401525, +254
              774 768 110 <br />
              EMAIL: sales@medilaballied.com info@medilaballied.com <br />

              medilab.alliedproductsltd@gmail.co
            </p>
          </div>
        </div>
      </v-flex>
      <div class="tfcontent-item" id="products">
        <span>Product Range</span>
        <div class="products">
          <div class="products-item"><a href="#">Kitchen Hygiene</a></div>
          <div class="products-item"><a href="#">House Keeping</a></div>
          <div class="products-item"><a href="#">Food & Beverage</a></div>
          <div class="products-item"><a href="#">Conveyor System</a></div>
          <div class="products-item"><a href="#">Personal Care</a></div>
          <div class="products-item"><a href="#">Workshop</a></div>
          <div class="products-item"><a href="#">Laundry</a></div>
          <div class="products-item"><a href="#">Water Treatmenr</a></div>
          <div class="products-item"><a href="#">Specialities</a></div>
        </div>
      </div>
      <div class="tfcontent-item" id="olinks">
        <span>Other Links</span>
        <div class="other-links">
          <div class="other-links-items"><a href="">About Us</a></div>
          <div class="other-links-items"><a href="">Contact Us</a></div>
          <div class="other-links-items"><a href="">Services</a></div>
          <div class="other-links-items"><a href="">Careers</a></div>
        </div>
      </div>
      <div class="tfcontent-item" id="nsform">
        <span>Subscribe to newsletter</span>
        <form action="">
          <div class="modal-name">
            <input type="text" name="name" placeholder="First Name" />
            <input type="text" name="name" placeholder="Surname" />
          </div>
          <div class="email">
            <input type="email" placeholder="Email adress or name" />
          </div>
          <v-btn
            success
            id="button"
            type="button"
            lable="Submit"
            style="top:20px; background:white; padding:10px 20px; color:blue; text-transform:lowercase;"
            >Subscribe</v-btn
          >
        </form>
      </div>
    </div>
  </v-layout>
</template>
<script>
export default {
  name: "topfooter"
};
</script>
<style scoped>
.tfcontent {
  color: #fff;

  font-weight: 700;
  font-size: 24px;
  position: relative;
  text-align: center;
  border-bottom: 3px solid transparent;
  display: grid;
  gap: 3em;
  left: 0;
  padding: auto;
}
a {
  text-decoration: none;
  color: white;
}
.tfcontent-item {
  color: #fff;
  padding: 10px 50px;
  position: relative;
  text-align: center;
  border-bottom: 1px solid transparent;
  display: flex;
  float: right;
  transition: width 4.4s;
}
#contactus {
  font-size: 24px;
  font-weight: 700;
  flex-direction: column;
}

#contacts {
  font-size: 12px;
  font-weight: 300;
  display: block;
  line-height: 30px;
  text-align: left;
}
#products {
  display: block;
}
.products {
  font-size: 12px;
  font-weight: 300;
  display: block;
  color: inherit;
  line-height: 30px;
  text-align: left;
}
#olinks {
  display: block;
}
.other-links {
  font-size: 12px;
  font-weight: 300;
  display: block;
  line-height: 30px;
  text-align: left;
}
#nsform {
  display: block;
}
form {
  display: block;
  padding: 20px 5px;
}
input[type="email"] {
  width: 100%;
  padding: 8px;
  font-size: 17px;
  border: none;
  border: 1px #ccc solid;
  border-radius: 5px;
  background: white;
}
input[type="text"] {
  width: inherit;
  padding: 8px 10px;
  font-size: 17px;
  border: none;
  border: 1px #ccc solid;
  border-radius: 5px;
  background: white;
}
.email {
  margin-top: 20px;
  width: 100%;
}
@media screen and (max-width: 950px) {
  .tfcontent {
    display: block;
  }
}
</style>
