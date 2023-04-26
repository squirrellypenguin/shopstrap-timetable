<template>
  <div class="home">
  <div class="container">
  <Media />
  </div>
  
  <div class="caption" >
    <div class="sign">
    <h1 class="title">Island Craft Shop</h1>
 
    <p class="lead" >An artisan cooperative</p>
  </div>
  <hr class="my-4">
  <p>The Island Craft Shop (ICS) located in the South Hero Village is the oldest artisan cooperative in the Lake Champlain Region</p>
  
  <div class="" >
  <div class="column conditional">
  <p></p>
  </div>
  <div class="column text-center justify-content-center ">
    <br>
    <br>
    <p class="lead ">
  <a class="centeredbtn btn-primary btn-lg" href="#/about" role="button" style="font-weight: bold; letter-spacing: .1rem;">Learn more</a>
  </p>
  </div>
  </div>
  </div>
  <div class="notes">
  </div>

</div>

</template>
<style scoped>

</style>
<script>
// @ is an alias to /src
import Media from './Media.vue'
export default {
  name: 'Home',
  components: {
          Media
  }
}
</script>
