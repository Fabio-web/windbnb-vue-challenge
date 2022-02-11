<template>
   <div class="homePage">
      <div class="titlePage">
         <h2>Stays in Finland</h2>
         <span>+{{ properties.length }} stays</span>
      </div>
      <div class="properties">
         <div class="property" v-for="(property, key) in properties" :key="key">
            <div class="thumbnail">
               <img :src="property.photo" :alt="property.title">
            </div>
            <div class="infos">
               <div class="details">
                  <div class="type">
                     <div class="tag" v-if="property.superHost">super host</div>
                     {{ property.type }}
                  </div>
                  <div class="rate">
                     <span class="material-icons-round">star_rate</span>
                     {{ property.rating }}
                  </div>
               </div>
               <div class="title">{{ property.title }}</div>
            </div>
         </div>
      </div>
   </div>
</template>

<style lang="scss">
@import "~/assets/scss/pages/home";
</style>

<script>
import stays from '../data/stays.json'

export default {
   head: {
      title: "Home"
   },
   data() {
      return {
         properties: stays
      }
   }
}
</script>
