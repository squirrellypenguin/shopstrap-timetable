<template>
  <div class="home">
  <div class="container">
  <Media />
  </div>
  
  <div class="caption" >
    <div class="sign front">
      <div contenteditable>
      <p class="title"><span style="color: #bf1b2c">I</span>sland <span style="color: #bf1b2c">C</span>raft <span style="color: #bf1b2c">S</span>hop</p>
    </div>
    <p class="lead" >A Cooperative Community</p>
    
    

  </div>
  <hr class="my-4">
  
  <p class="middle-picket" >located in the South Hero Village</p> 
  <p class="btm-picket"><span style="padding: 3px; background-color: white">The oldest artisan cooperative in the Lake Champlain Region</span></p>
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
