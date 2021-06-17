<template>
  <div class="home">
    <div class="carousel">
      <VueSlickCarousel v-bind="settings">
        <div><h1>1</h1></div>
        <div><h1>2</h1></div>
        <div><h1>3</h1></div>
        <div><h1>4</h1></div>
        <div><h1>5</h1></div>
        <div><h1>6</h1></div>
      </VueSlickCarousel>
    </div>
  </div>
</template>

<style>
.carousel {
  background: #eeeeee;
  max-width: 50%;
  margin: auto;
  padding: 50px;
}
</style>

<script>
import VueSlickCarousel from "vue-slick-carousel";
import "vue-slick-carousel/dist/vue-slick-carousel.css";
// optional style for arrows & dots
import "vue-slick-carousel/dist/vue-slick-carousel-theme.css";

export default {
  data: function () {
    return {
      settings: {
        arrows: true,
        dots: true,
        dotsClass: "slick-dots",
        edgeFriction: 0.75,
        infinite: true,
        speed: 250,
        slidesToShow: 1,
        slidesToScroll: 1,
        autoplay: true,
        pauseOnDotsHover: true,
        draggable: true,
        focusOnSelect: true,
      },
    };
  },
  name: "MyComponent",
  components: { VueSlickCarousel },

  methods: {},
};
</script>
