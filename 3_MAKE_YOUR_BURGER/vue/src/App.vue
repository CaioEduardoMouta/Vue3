<template>
  <NavBar :logo="logo_src" :alt="app_name"/>
  <BannerComponents />
  <router-view/>
  <FooTer />
</template>
  
<script>

import NavBar from "./components/NavBar.vue";
import FooTer from "./components/FooTer.vue";
import BannerComponents from "./components/BannerComponents.vue";

export default {

  components: {
    NavBar,
    FooTer,
    BannerComponents
},
data() {
  return {
    logo_src: "/img/logo.png",
    app_name: "Make Your Burguer"
  }
}
}

</script>

<style>

* {
  font-family: Helvetica;
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

.main-container {
  margin: 50px;
  min-height: 250px;
}

h1 {
  text-align: center;
  font-size: 42px;
  margin-bottom: 30px;
  color: #222;
}
</style>
