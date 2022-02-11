<template>
   <div id="app">
      <Header/>
      <div class="container">
         <Nuxt/>
      </div>
      <Footer/>
   </div>
</template>

<script>
import Vue from "vue"
import Header from "../components/layouts/header"
import Footer from "~/components/layouts/footer"

export default Vue.extend({
   layout: "default",
   components: { Footer, Header }
})
</script>
