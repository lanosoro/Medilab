<template>
  <footer class="footer">
    <div class="container">
      <div class="row">
        <div class="footer-col">
          <h4>
            Why Medilabs Ltd
          </h4>
          <p style="color:white;">
            We believe "Quality is not an act, it is a Habit,” Committed to
            develop, sustain high quality in manufacturing of drug formulations
            in order to meet the customers satisfaction.
          </p>
        </div>
        <div class="footer-col">
          <h4>
            Our Main Goal
          </h4>
          <p style="color:white;">
            Medilabs main goal is to provide quality healthcare to all through a
            wide range of healthcare products that meet individual customer
            needs.
          </p>
        </div>
        <div class="footer-col">
          <h4>
            other Links
          </h4>
          <ul>
            <li><a href="#">About Us</a></li>
            <li><a href="#">Contact Us</a></li>
            <li><a href="#">Services</a></li>
            <li><a href="#">Careers</a></li>
          </ul>
        </div>
        <div class="footer-col">
          <h4>
            follow Us
          </h4>
          <div class="social-links">
            <a href="#"><i class="fab fa-facebook-f"></i></a>
            <a href="#"><i class="fab fa-twitter"></i></a>
            <a href="#"><i class="fab fa-instagram"></i></a>
            <a href="#"><i class="fab fa-linkedin-in"></i></a>
          </div>
          <form action="#">
            <input type="email" name="email" placeholder="email" id="" />
            <input type="button" value="" />
          </form>
        </div>
      </div>
    </div>
    <div id="bottomfooter">
      Copyright © {{ new Date().getFullYear() }}· All Rights Reserved · Medilabs
      Ltd Web design by ·<span id="link">
        <a href="http://fineteklabs.com"> Finetek</a>
      </span>
    </div>
  </footer>
</template>

<script>
export default {};
</script>

<style scoped>
.footer {
  background-color: #0074a5;
  padding: 60px 60px 0px 0px;
  widows: 100vw;
}
#footer {
  bottom: 0;
  width: 100%;
}
#link {
  text-decoration: none;
  color: inherit;
  transition: cubic-bezier(0.075, 0.82, 0.165, 1) 0.5s ease-in-out;
}
#link::before {
  font-size: 28px;
}
#link::after {
  font-size: 18px;
}
#bottomfooter {
  position: relative;
  left: 0;
  right: 0;
  background: #28b6e7;
  width: 100vw;
  padding: 30px;
  margin-left: 0;
  color: white;
  font-weight: 400;
  font-size: 18px;
  justify-content: center;
  text-align: center;
  margin-top: 70px;
}
.container {
  max-width: 1170px;

  margin: auto;
}
.footer-col {
  width: 25%;
  padding: 0 35px;
}
.footer-col h4 {
  font-size: 28px;
  color: inherit;
  text-transform: capitalize;
  margin-bottom: 35px;
  font-weight: 700;
  position: relative;
}
.footer-col h4::before {
  content: "";
  position: absolute;
  left: 0%;
  bottom: -10px;
  background: white;
  height: 2px;
  box-sizing: border-box;
  width: 150px;
}
.footer-col ul li:not(:last-child) {
  margin-bottom: 10px;
}
.footer-col ul li a {
  font-size: 16px;
  text-transform: capitalize;
  font-weight: 300;
  display: block;
  text-decoration: none;
}
.footer-col ul li a:hover {
  padding: 8px;

  font-size: 19px;
  shadow: rgba(0, 0, 0, 0.4);
  transition: all 0.3s ease-in-out;
}
ul {
  list-style: none;
}
a {
  text-decoration: none;
  color: white;
}
.row {
  display: flex;
  flex-wrap: wrap;
}
.footer-col .social-links a {
  display: inline-block;
  height: 40px;
  width: 40px;
  background-color: rgba(255, 255, 255, 0.2);
  border-radius: 50%;
  margin: 0 10px 10px 0;
  text-align: center;
  line-height: 40px;
  transition: all 1s ease;
}
.footer-col .social-links a:hover {
  background: white;
  color: #0074a5;
}
/*responsive */
@media (max-width: 767px) {
  .footer-col {
    width: 50%;
    padding: 0 15px;
    margin-bottom: 30px;
    font-size: 14px;
  }
  .container {
    max-width: 100%;

    margin: auto;
  }

  .container #bottmfooter {
    max-width: 100%;
    position: relative;
    left: -10;
    right: 0;
    background: #28b6e7;

    padding: 30px;
    margin-right: 0;
    margin: auto;
  }
  #bottomfooter {
  }
}
@media (max-width: 574px) {
  .footer-col {
    width: 100%;
    font-size: 14px;
  }
  .container {
    max-width: 100%;
  }
  .footer {
    padding: 0px 0px;

    font-size: 14px;
    text-align: center;
  }
  .container #bottomfooter {
    max-width: 100%;
    position: relative;
    left: -10;
    right: 0;
    background: #28b6e7;

    padding: 30px;
    margin-right: 0;
  }
  #bottomfooter {
    position: relative;
    left: 0;
    right: 0;
    font-size: 12px;
    max-width: 100%;
    padding: 30px;
  }
  .footer-col h4 {
    font-size: 28px;
    color: white;
    text-transform: capitalize;
    margin-bottom: 35px;
    font-weight: 700;
    position: relative;
  }
  .footer-col h4::before {
    content: "";
    position: absolute;
    left: 28%;
    bottom: -10px;
    background: white;
    height: 2px;
    box-sizing: border-box;
    width: 150px;
  }
}
</style>
