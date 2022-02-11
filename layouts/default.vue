<template>
   <div id="app">
      <Nuxt/>
   </div>
</template>

<style lang="scss">
@import "@/assets/scss/app.scss";
</style>

<script>
import Vue from "vue"
import Header from "../components/layouts/header"

export default Vue.extend({
   layout: "default",
   components: { Header }
})
</script>
