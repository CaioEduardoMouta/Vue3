<template>
  <NavBar :logo="logo_src" :alt="app_name"/>
  <router-view/>
  <FooTer />
</template>
  
<script>

import NavBar from "./components/NavBar.vue";
import FooTer from "./components/FooTer.vue";

export default {

  components: {
    NavBar,
    FooTer
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

</style>
