<template>
<div class="container">
  <nav>Navbar</nav>
  <main>
     <div id="content1">
    <div>
          <img
            src="https://www.odexchemicals.com/wp-content/uploads/2019/08/housekeepingicon.png"
            alt=""
          />
        </div>
  </div>
  <div id="content2"><div>
          <img
            src="https://www.odexchemicals.com/wp-content/uploads/2019/08/watertreatmenticon.png"
            alt=""
          />
        </div></div>
  <div id="content3">
    <div id="d" style="top:30px; position:relative;">
          <img
            src="https://www.odexchemicals.com/wp-content/uploads/2019/08/conveyorsystemsicon.png"
            alt=""
          />
        </div>
  </div>
  </main>
  <div id="sidebar">Our Product Range</div>
  <div id="content1">
    <div>
          <img
            src="https://www.odexchemicals.com/wp-content/uploads/2019/08/housekeepingicon.png"
            alt=""
          />
        </div>
  </div>
  <div id="content2"><div>
          <img
            src="https://www.odexchemicals.com/wp-content/uploads/2019/08/watertreatmenticon.png"
            alt=""
          />
        </div></div>
  <div id="content3">
    <div id="d" style="top:30px; position:relative;">
          <img
            src="https://www.odexchemicals.com/wp-content/uploads/2019/08/conveyorsystemsicon.png"
            alt=""
          />
        </div>
  </div>
  <footer>Footer</footer>
</div>

</template>

<script>
export default {

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

.container {
  display: grid;
  height: 100vh;
  grid-template-columns: 1fr 1fr 1fr 1fr;
  grid-template-rows: 0.2fr 1.5fr 1.2fr 0.8fr;
  grid-template-areas:
    "nav nav nav nav"
    "sidebar main main main "
    "sidebar content1 content2 content3 "
    "footer footer footer footer";
  grid-gap: 0.44rem;
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
  display: none;
}

main {
  background: #84ffff;
  grid-area: main;
  border-radius: var(--main-radius);
  padding-top: var(--main-padding);
  display: flex;
  flex-direction: row;
}

#sidebar {
  background: #28b6e7;
  color: white;
  padding: 15px 90px;
  font-size: 25px;
  grid-area: sidebar;
  border-radius:10px;
  padding-top: var(--main-padding);

}

#content1 {

  grid-area: content1;
  background-color: #f2f2f2;
  border-radius: 10px;
  margin: 1%;
  text-align: center;
  display: flex;
  flex-direction: column;
  padding: 20px;
}

#content2 {

  grid-area: content2;
  
  background-color: #f2f2f2;
  border-radius: 10px;
  margin: 1%;
  text-align: center;
  display: flex;
  flex-direction: column;
  padding: 20px;
}

#content3 {
   grid-area: content3;
  
  background-color: #f2f2f2;
  border-radius: 10px;
  margin: 1%;
  text-align: center;
  display: flex;
  align-items: center;
  flex-direction: column;
  padding: 20px;
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
      "main"
      "content1"
      "content2"
      "content3"
      "footer";
  }
}


</style>