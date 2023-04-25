<template>
<div>
  <div id="app">
      <div id="nav">
        <Header />
      </div>
      <router-view/>
  </div>
  <footer class="footer">
  <div class="row">
  <a href="https://www.facebook.com/Island-Craft-Shop-189477107771345/" alt="FB" style="color:white"><font-awesome-icon :icon="{ prefix: 'fab', iconName: 'facebook' }"/></a>
  <a href="https://www.instagram.com/vtislandcraftshop" alt="insta" style="color:white"><font-awesome-icon :icon="{ prefix: 'fab', iconName: 'instagram' }"/></a>
  <a href="https://www.instagram.com/vtislandcraftshop" alt="twitter" style="color:white"><font-awesome-icon color:white :icon="{ prefix: 'fab', iconName: 'twitter' }"/></a>
  <div style="color: white; font-size:12px"><p>Tel: (802) 372-3945</p>
    <p>
  329 U.S. Rte 2, South Hero, VT 05486</p>
</div>
  </div>
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