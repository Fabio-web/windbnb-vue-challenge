<template>
   <header>
      <div class="container">
         <nuxt-link to="/" class="icon">
            <img src="~/assets/images/logo.svg" alt="windbnb icon">
         </nuxt-link>
         <div class="search">
            <div class="location">Helsinki, Finland</div>
            <div class="guests placeholder">Add guest</div>
            <div class="material-icons">search</div>
         </div>
      </div>
   </header>
</template>

<style lang="scss">
@import "style";
</style>

<script>
import Vue from "vue"

export default Vue.extend({
   name: "Header"
})
</script>
