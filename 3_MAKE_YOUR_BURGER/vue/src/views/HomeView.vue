<template>
  <BannerComponents />
 <div class="main-container">
    <h1>Monte seu Burger:</h1>
    <BurgerForm />
 </div>
</template>

<script>
import BannerVue from "../components/BannerComponents.vue"
import BurgerForm from "@/components/BurgerForm.vue"

export default {
  name: "nome",
  components: {
    BannerVue,
    BurgerForm,

}
}

</script>
