<template>
  <footer class="footer">
      <div class="container">
          <div class="row">
          <div class="footer-col">
              <h4>
                  company
              </h4>
              <ul>
                  <li><a href="#">about us</a></li>
                  <li><a href="#">our survey</a></li>
                  <li><a href="#">privacy policy</a></li>
                  <li><a href="#">affiliatie proram</a></li>
              </ul>
          </div>
           <div class="footer-col">
              <h4>
                  get help
              </h4>
              <ul>
                  <li><a href="#">FAAQ</a></li>
                  <li><a href="#">shipping</a></li>
                  <li><a href="#">returns</a></li>
                  <li><a href="#">Order Status</a></li>
                  <li><a href="#">payment options</a></li>
              </ul>
          </div> <div class="footer-col">
              <h4>
                  online shop
              </h4>
              <ul>
                  <li><a href="#">watch</a></li>
                  <li><a href="#">bag</a></li>
                  <li><a href="#">blash</a></li>
                  <li><a href="#">dress</a></li>
              </ul>
          </div> <div class="footer-col">
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
                  <input type="email" name="email" placeholder="email" id="">
                  <input type="button" value="">
              </form>
          </div></div>
      </div>
<div id="bottomfooter"></div>
  </footer>
</template>

<script>

export default {

}
</script>

<style scoped>
 
.footer{
    background-color:#0074a5 ;
    padding: 60px 60px 0px 0px;
    widows: 100vw;
    

    
}
#footer{
    bottom: 0;
    width: 100%;

}
#bottomfooter {
  position: relative;
  left: 0;
  right: 0;
  background: #28b6e7;
  width: 100vw;
  padding: 30px;
  margin-left: 0;
}
.container{
    max-width: 1170px;
    
    margin: auto;

}
.footer-col{
    width: 25%;
    padding: 0 15px;


}
.footer-col h4{
    font-size: 28px;
    color: inherit;
    text-transform: capitalize;
    margin-bottom: 35px;
    font-weight: 700;
    position: relative;
   

}
.footer-col h4::before{
    content: '';
    position: absolute;
    left: 0%;
    bottom: -10px;
    background: white;
    height: 2px;
    box-sizing: border-box;
    width: 150px;

}
.footer-col ul li:not(:last-child){
    margin-bottom: 10px;
}
.footer-col ul li a{
    font-size: 16px;
    text-transform: capitalize;
    font-weight: 300;
    display: block;
    text-decoration: none;


}
.footer-col ul li a:hover{
    padding: 8px;
    
    font-size: 19px;
    shadow: rgba(0, 0, 0, 0.4);
    transition:all 0.3s ease-in-out;
}
ul{
    list-style: none;
}
a
{
    text-decoration: none;
    color: white;
}
.row{
    display: flex;
    flex-wrap: wrap;
}
.footer-col .social-links a{
    display: inline-block;
    height: 40px;
    width: 40px;
    background-color:rgba(255, 255,255, 0.2) ;
    border-radius: 50%;
    margin:0 10px 10px 0;
    text-align: center;
    line-height: 40px;
    transition: all 1s ease;
}
.footer-col .social-links a:hover{
    background:white;
    color: #0074a5;
}
/*responsive */
@media  (max-width:767px) 
{
    .footer-col{
    width: 50%;
    padding: 0 15px;
    margin-bottom:30px ;


}
.container{
    max-width: 100%;
    
    margin: auto;


}
.container #bottmfooter{
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
@media  (max-width:574px) 
{
    .footer-col{
    width: 100%;
   


}
.container{
    max-width: 100%;

   


}
.container #bottomfooter{
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

  max-width: 100%;
  padding: 30px;
}
}
</style>