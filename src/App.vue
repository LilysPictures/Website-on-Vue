<template>

<div id="app">
  <app-header/>
  <spider/>
 
  <!-- <router-link to="/"> HOME </router-link> -->
  <!-- <span class="Osya" @click="click">
  <router-link :to="{name: 'Osya'}"> <img src="./assets/Osya.png" alt="Osya" style="width: 300px; height: 300px; position: absolute; z-index: 12000"> </router-link> 
  </span> -->
  <!-- <router-link :to="{name: 'Header'}"> Header </router-link> -->

  <router-view/>
  <ghost/>
  <app-footer/>
</div>

</template>

<script>


import AppHeader from '@/layouts/AppHeader'
import AppFooter from '@/layouts/AppFooter'
import spider from '@/components/spider'
import ghost from '@/components/ghost'

export default {
   name: "App",
  data() {
    return {
    }
  },

components: {AppHeader, AppFooter, spider, ghost},

}


</script>

<style>
*, :after, :before {
    box-sizing: border-box;
    margin: 0;
}
#app {
  font-family: 'Frijole', cursive;
  position: relative;
  height: 100vh;
  margin: 0; 
  background: url(./assets/BG_MM.jpg) center no-repeat fixed;
  background-size: cover;
  
}


</style>
