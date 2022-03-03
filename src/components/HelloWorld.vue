<template>
  <div class="sliderbase">
  <carousel :items-to-show="6" :itemsToScroll="1">
    <slide class="bgcolor" v-for="slide in 10" :key="slide">
      <div class="carousel__item">{{ slide }}</div>
    </slide>

    <template #addons>
      <navigation />
      <pagination />
    </template>
  </carousel>
  </div>
</template>

<script>
import 'vue3-carousel/dist/carousel.css';
import { Carousel, Slide, Pagination, Navigation } from 'vue3-carousel';
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  components: {
    Carousel,
    Slide,
    Pagination,
    Navigation,
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.sliderbase{
  width: 50%;
  margin: 0 auto;
}
.bgcolor{
  background-color: cadetblue;
}
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
