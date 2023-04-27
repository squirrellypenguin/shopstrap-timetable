

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
                      <!-- Title -->
                        <h3 class="text-black fs-5">{{artist.name}}</h3>
                      
                      <!-- Business name -->
                        <p>{{artist.dba}}</p>

                      <!-- About me -->
                        <p class="fs-6 text-black">{{artist.artistStatement}}</p>
                    
                          
                      <!-- Website -->
                      <a :href="artist.website" alt="homepage" style="color:black; padding-right: 10px;"><font-awesome-icon color:black :icon="{ prefix: 'fa', iconName: 'home' }"/></a>  

                      <!-- Twitter Link -->
                        <a :href="artist.twitter" alt="twitter" style="color:black; padding-right: 10px;"><font-awesome-icon :icon="{ prefix: 'fab', iconName: 'twitter' }"/></a>
                    
                        
                      <!-- Facebook Link -->
                        <a class="link-light" :href="artist.facebook" alt="FB" style="color:black; padding-right: 10px;"><font-awesome-icon :icon="{ prefix: 'fab', iconName: 'facebook' }"/></a>
                       
                      <!-- Squarestore Link -->
                        <a class="link-light" :href="artist.SquareStore" alt="squareB" style="color:black; padding-right: 10px;"><font-awesome-icon :icon="{ prefix: 'fa', iconName: 'square'}"/></a>
                       
                       
                      <!-- Instragram Link -->
                        <a :href="artist.Instagram" alt="insta" style="color:black; padding-right: 10px;"><font-awesome-icon :icon="{ prefix: 'fab', iconName: 'instagram' }"/></a>
                       
                    
                      <!-- Esty Store -->
                       <a :href="artist.EtsayStore" alt="etsy" style="color:black; padding-right: 10px;"><font-awesome-icon :icon="{ prefix: 'fab', iconName: 'etsy' }"/></a>
                        
                      <!-- Email -->
                        <a v-bind:href="'mailto:' + artist.email">
                        <i style="color:black;" class="fa fa-paper-plane" aria-hidden="true"></i> </a>

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