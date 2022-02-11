<template>
   <header>
      <div class="container">
         <nuxt-link to="/" class="icon">
            <img src="~/assets/images/logo.svg" alt="windbnb icon">
         </nuxt-link>
         <div class="search" @click="toggleSearch">
            <div class="location">Helsinki, Finland</div>
            <div class="guests placeholder">Add guest</div>
            <div class="material-icons">search</div>
         </div>
      </div>
      <Search/>
   </header>
</template>

<style lang="scss">
@import "style";
</style>

<script>
import Vue from "vue"
import Search from "~/components/search"

export default Vue.extend({
   name: "Header",
   components: { Search },
   methods: {
      toggleSearch() {
         this.$nuxt.$emit("search")
      }
   }
})
</script>
