<template>
  <v-layout class="container">
  <div class="content4">
      <span id="java">
          Our Product Range
      </span>
  </div>
   <div class="productcontainer" >
       <div class="productcategory"  >
           <div class="productimage" >
               <img src="https://www.odexchemicals.com/wp-content/uploads/2019/08/kitchenhygieneicon.png" alt="">
           </div>
       </div>
        <div class="productcategory"   >
           <div  >
               <img src="https://www.odexchemicals.com/wp-content/uploads/2019/08/kitchenhygieneicon.png" alt="">
           </div>
       </div>
        <div class="productcategory"  >
           <div  >
               <img src="https://www.odexchemicals.com/wp-content/uploads/2019/08/kitchenhygieneicon.png" alt="">
           </div>
       </div> <br>
        <div id="content5" class="productcategory"  >
           <div id="d" >
               <img src="https://www.odexchemicals.com/wp-content/uploads/2019/08/kitchenhygieneicon.png" alt="">
           </div>
       </div>
        <div class="productcategory"  >
           <div class="productimage" >
               <img src="https://www.odexchemicals.com/wp-content/uploads/2019/08/kitchenhygieneicon.png" alt="">
           </div>
       </div>
        <div class="productcategory"  >
           <div class="productimage" >
               <img src="https://www.odexchemicals.com/wp-content/uploads/2019/08/kitchenhygieneicon.png" alt="">
           </div>
       </div>
        <div class="productcategory"  >
           <div class="productimage" >
               <img src="https://www.odexchemicals.com/wp-content/uploads/2019/08/kitchenhygieneicon.png" alt="">
           </div>
       </div>
   </div>
  <main>
    <div class="contents">

    </div>
  </main>
 
 <footer></footer>
  </v-layout>

</template>

<script>
export default {
       data(){
        return{
            slides:[
                {
                    src:"https://www.odexchemicals.com/wp-content/uploads/2019/08/kitchenhygieneicon.png"
                },
                {
                    src:"https://www.odexchemicals.com/wp-content/uploads/2019/08/housekeepingicon.png"
                },
                {
                    src:"https://www.odexchemicals.com/wp-content/uploads/2019/08/foodbeverageicon.png"
                }
            ]
        }
    }

}
</script>

<style scoped>
:root {
  --main-radius: 5px;
  --main-padding: 5px;
}

body {
  font-family: "Inter", sans-serif;
}
.productcontainer{
   
    flex-direction: row;
    float: right;
    padding: 0px 30px;
    height: 400px;
    width: 60vw;
    margin: 30px;
    display: flex;
    justify-content: flex-start;
    flex-wrap: wrap;
    flex-grow: 1;
    overflow-y:hidden ;
}
.productcategory{
    width: 18%;
    background-color: #f2f2f2;
    border-radius: 10px;
    margin: 1%;
    text-align: center;
    display: flex;
    flex-direction: column;
    padding: 20px;
}

.container {
  display: grid;
  height: 100vh;
  width: 100vw;
  grid-template-columns: 1fr 1fr 1fr 1fr;
  grid-template-rows: 1.5fr 1.2fr 0.8fr;
  grid-template-areas:

    "content4 productcontainer productcontainer content3"
    "content4 content5 content6 content7"
    "main main main main"
    
    "sidebar footer footer footer";
  grid-gap: 0.2rem;
  font-weight: 800;
  text-transform: uppercase;
  font-size: 12px;
  color: #004d40;
  text-align: center;
}

nav {
  background: #a7ffeb;
  grid-area: nav;
  border-radius: var(--main-radius);
  padding-top: var(--main-padding);
}

main {
  background: #84ffff;
  grid-area: main;
  border-radius: var(--main-radius);
  padding-top: var(--main-padding);
}

#sidebar {
  background: #18ffff;
  grid-area: sidebar;
  border-radius: var(--main-radius);
  padding-top: var(--main-padding);
}

#content1 {
  background: #6fffd2;
  grid-area: content1;
  border-radius: var(--main-radius);
  padding-top: var(--main-padding);
}

#content2 {
  background: #64ffda;
  grid-area: content2;
  border-radius: var(--main-radius);
  padding-top: var(--main-padding);
}

#content3 {
  background: #73ffba;
  grid-area: content3;
  border-radius: var(--main-radius);
  padding-top: var(--main-padding);
}
.content4{
  background: #28b6e7;
  grid-area: content4;
  padding: 30px;
  border-radius: 10px;
  color: white;
  font-size: 32px;
  padding-top: var(--main-padding);
}
#java{
    position: relative;
    bottom: 0;
}

footer {
  background: #1de9b6;
  grid-area: footer;
  border-radius: var(--main-radius);
  padding-top: var(--main-padding);
}

a {
  text-align: center;
  display: block;
  font-family: inherit;
  text-decoration: none;
  font-weight: bold;
  margin: 1rem;
}

@media only screen and (max-width: 550px) {
  .container {
    grid-template-columns: 1fr;
    grid-template-rows: 0.4fr 0.4fr 2.2fr 1.2fr 1.2fr 1.2fr 1fr;
    grid-template-areas:
      "nav"
      "sidebar"
      "content4"
      "content1"
      "content2"
      "content3"
      "footer";
  }
.productcontainer{
   
    flex-direction: column;
    padding: 0px 30px;
    height: 300px;
    width: 50%;
    margin: 10px;
    display: block;
    justify-content: flex-start;
    flex-wrap: wrap;
    flex-grow: 1;
}
.productcategory{
    width: 18%;
    background-color: #f2f2f2;
    border-radius: 10px;
   
    text-align: center;
    display: block;
    flex-direction: column;
    padding: 20px;
}
#content4{
  position: relative;
  top: 0px;
}
}

</style>