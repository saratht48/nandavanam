<template>
  <splide :options="options">
    <splide-slide>
      <div class="sliderdata"></div>
    </splide-slide>
    <splide-slide>
      <div class="sliderdata"></div>
    </splide-slide>
    <splide-slide>
      <div class="sliderdata"></div>
    </splide-slide>
    <splide-slide>
      <div class="sliderdata"></div>
    </splide-slide>
    <splide-slide>
      <div class="sliderdata"></div>
    </splide-slide>
    <splide-slide>
      <div class="sliderdata"></div>
    </splide-slide>
  </splide>
</template>


<script>
import { Splide, SplideSlide } from '@splidejs/vue-splide';
import '@splidejs/splide/dist/css/themes/splide-default.min.css';
export default {
  name: 'HelloWorld',
  data() {
      return {
        options: {
          rewind : true,
          gap    : '1rem',
          perPage: 5,
        },
      };
    },
  props: {
    msg: String
  },
  components: {
    Splide,
    SplideSlide,
  },
}
</script>

<style scoped>
.sliderdata{
  width: 100%;
  height: 250px;
  background-color: red;
}
</style>