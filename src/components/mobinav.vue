<template>
  <section class="nav">
    <div class="nav-menu">
      <div class="nav-menu-list">
        <a href="" id="careers">Careers</a>

        <v-autocomplete
          id="search"
          v-model="model"
          :items="items"
          :loading="isLoading"
          :search-input.sync="search"
          chips
          clearable
          hide-details
          hide-selected
          item-text="name"
          item-value="symbol"
          label="Search ..."
          solo
          style="width:300px; position:relative; right:30px"
        ></v-autocomplete>
      </div>
    </div>
  </section>
</template>
<style scoped>
.nav {
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  align-items: flex-end;
}
.nav-logo {
  display: none;
}
.search {
  z-index: 1000000;
  padding: 10px;
  background: white;
  border-radius: 10px;
}
.avatar {
  border-radius: 50%;
  width: 60px;
}
.nav-menu-list {

  padding: 10px;
  display: flex;
  flex-direction: row;
  margin: 0;
  color: white;
  border-spacing: 12px;
}
li {
}
li:hover {
  background: #333;
}
li:first-of-type {
}
a {
  position: relative;
  text-decoration: none;
  color: white;
  font-size: 0.889em;
  right: 50px;
  top: 12px;
}
li:nth-last-of-type(2) {
  border-bottom: 5px solid #222;
}
@media screen and (max-width: 950px) {
  #search {
    width: 70vw;
  }
  #careers {
    display: none;
  }
}
</style>
