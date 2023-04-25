<template>
<div>
  <div id="app">
      <div id="nav">
        <Header />
      </div>
      <router-view/>
  </div>
  <footer class="footer">
  <div style="width:300px;" class="row">
  <a class="link-light" href="https://www.facebook.com/Island-Craft-Shop-189477107771345/" alt="FB" style="color:white; padding-right: 10px;"><font-awesome-icon :icon="{ prefix: 'fab', iconName: 'facebook' }"/></a>
  <a href="https://www.instagram.com/vtislandcraftshop" alt="insta" style="color:white; padding-right: 10px;"><font-awesome-icon :icon="{ prefix: 'fab', iconName: 'instagram' }"/></a>
  <a href="https://www.instagram.com/vtislandcraftshop" alt="twitter" style="color:white; padding-right: 10px;"><font-awesome-icon color:white :icon="{ prefix: 'fab', iconName: 'twitter' }"/></a>
  <div style="color: white; font-size:12px; padding-top: 10px;"><a style="color:white" href="tel:8023723945">Call us @ 802-372-3945</a></div></div>
  <p style="color: white; font-size:14px">Find us @ 329 U.S. Rte 2, South Hero, VT 05486</p>
  </footer>
  </div>
</template>

<style lang="scss">

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}


</style>
<script>
import Header from '@/components/Header.vue'

export default {
  name: 'Home',
  components: {
    Header
  }
}
</script>