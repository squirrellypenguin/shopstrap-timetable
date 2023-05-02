<template>
<div>


  <splide :options="options">
    <splide-slide>
      <p><img width="1600" height="900"  class="resposnive" src="https://res.cloudinary.com/doammukzv/image/upload/v1682682860/Art/Halstrom6_zdisrz.jpg" /> </p>
    </splide-slide>
    <splide-slide>
      <p><img  width="1600" height="900"  class="resposnive" src="https://res.cloudinary.com/doammukzv/image/upload/v1682931111/Little_Guys_1_twdlmj.jpg" /> </p>
    </splide-slide>
    <splide-slide>
      <p><img  width="1600" height="900" class="resposnive" src="https://res.cloudinary.com/doammukzv/image/upload/v1682682860/Art/Halstrom6_zdisrz.jpg" /> </p>
    </splide-slide>
  </splide>
  </div>
</template>

<script>
import { Splide, SplideSlide } from '@splidejs/vue-splide';
import '@splidejs/splide/dist/css/themes/splide-default.min.css';
export default {
  components: {
    Splide,
    SplideSlide,
  },
   data() {
      return {
        videoid: "nmsZRw-RWYI",
        options: {
          rewind : true,
          width: 1600,
          cover: true,
          gap: '1rem',
          autoplay: true,
          pauseOnHover: false,
          type  : 'fade',
          breakpoints: {
            980: {
              width: 700,
            },
           
            775: {
              width: 700,
            },
           
          },
        },
      };
    },
}

</script>
