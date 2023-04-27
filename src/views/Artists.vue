

<template>





  <div class="container-fluid">
   <div class="gallery"> 
    <div class="frame" v-for="(artist, index) in artists" :key=index>
    <div class="artist">
      <div class="container d-flex align-items-center justify-content-center flex-wrap">
        <div class="box">
            <div class="body">
            
                <div style="background-color:black;" class="imgContainer">
                  <p style="color:white; z-index: 100;">{{artist.name}}</p>
                    
                </div>
                <div class="content d-flex flex-column align-items-center justify-content-center">
                    <div>
                        <h3 class="text-white fs-5">Post Title</h3>
                        <p class="fs-6 text-white">Lorem ipsum dolor sit amet consectetur adipisicing elit. Explicabo sed cum neque, rem provident ex. Laboriosam perspiciatis modi eveniet in?</p>
                    </div>
                </div>
            </div>
        </div>

     
    </div>
      


    <!-- <div class=""><p>{{ artist.gsx$name.$t }}</p>
    <p>{{ artist.gsx$about.$t }}</p>
    </div>
    <div class=''>
    <div class="button-box">
    <button> <font-awesome-icon :icon="{ prefix: 'fas', iconName: 'door-closed' }"/>Website{{ artist.gsx$website.$t }}</button>
    <button><font-awesome-icon :icon="{ prefix: 'far', iconName: 'paper-plane' }" />Email{{ artist.gsx$email.$t }}</button>
    <button><font-awesome-icon :icon="{ prefix: 'fab', iconName: 'facebook' }"/>
{{ artist.gsx$facebook.$t }}</button> 
     </div> 
    </div>  -->
   </div>
   </div>
   </div>
 </div>
</template>

<script>
// @ is an alias to /src
import axios from 'axios';
export default {
  name: 'Artists',
  components: {
    
  },

 data() {
    return {
      artists: [],
      errors: []
    }
  },

  // Fetches posts when the component is created.
  async created() {
    try {
      const response = await axios.get('https://sheet.best/api/sheets/06fc3b51-300c-40ce-a5ef-76c218e62cdd')
      console.log(response.data[1])
      this.artists = response.data
     
    } catch (error) {
      this.errors.push(error)
    }
  }
}
</script>