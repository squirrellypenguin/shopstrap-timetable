<template>
  <div class="home">
  <div class="container">
  <Media />
  </div>
  <div class="caption" >
  <h1 class="title">Island Craft Shop</h1>
  <p class="lead" >An artisan cooperative</p>
  <hr class="my-4">
  <p>Island Craft Shop (ICS) located at 329 US Route 2 in South Hero Village is the oldest artisan cooperative in the Lake Champlain Region</p>
  
  <div class="row" >
  <div class="column conditional">
  <p>dsfsdfdsfdsfds</p>
  </div>
  <div class="column">
  <p class="lead">
  <a class="btn btn-primary btn-lg" href="#/about" role="button" style="font-weight: bold; letter-spacing: .1rem;">Learn more</a>
  </p>
  </div>
  </div>
  </div>
  <div class="notes">NOTES
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
