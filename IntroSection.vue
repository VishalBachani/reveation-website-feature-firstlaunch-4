<template>
 
<section class="rl-intro">
   <b-carousel
      id="carousel-1"
      :interval="4000"
      controls
      indicators
    >
      <!-- Text slides with image -->
      <b-carousel-slide
        caption="WE HELP LEADERS AND THEIR TEAMS MAKE INNOVATION HAPPEN"
        
        :img-src="require('@/assets/images/intro-carousel/1.jpg')"
      ></b-carousel-slide>

      <!-- Slides with custom text -->
      <b-carousel-slide :img-src="require('@/assets/images/intro-carousel/2.jpg')">
        <h1>A HOLISTIC APPROACH TO TRANSFORMING YOUR ORGANIZATION!     </h1>
      </b-carousel-slide>

      <!-- Slides with image and text  only -->
      <b-carousel-slide :img-src="require('@/assets/images/intro-carousel/3.jpg')">
          <h1>A PERFECT GATEWAY FOR ALL DIGITAL SOLUTIONS   </h1>
      </b-carousel-slide>

    </b-carousel>
</section>
</template>

<script>
export default {
  data() {
    return {
      message: "Try change me!"
    };
  },
  methods: {
    onClick() {
      this.message = "Here you go :)";
    }
  }
};
</script>

<style>
.rl-intro .carousel-item {
  height: 100vh;
  min-height: 350px;
  
  background: no-repeat center center scroll;
  -webkit-background-size: cover;
  -moz-background-size: cover;
  -o-background-size: cover;
  background-size: cover;
}
.rl-intro .carousel-item img {
    width: 100%;
    height: 100vh;
    object-fit: cover;
    object-position: center;    
}
.rl-intro .carousel-item:before {
  content: '';
  background-color: rgba(1, 0, 0, 0.7);
  position: absolute;
  height: 100%;
  width: 100%;
  top: 0;
  right: 0;
  left: 0;
  bottom: 0;
}
</style>