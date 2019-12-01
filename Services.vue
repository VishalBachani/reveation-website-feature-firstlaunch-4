<template>
  <section id="services" class="rl-services">
      <b-container>

        <header class="section-header fadeInUp" v-wow="{ 'animation-name': 'fadeInUp','animation-duration': '1s'}">
          <h3>Services</h3>
          <p></p>
        </header>

        <b-row>

            <b-col lg="4" md="6" class="box" v-wow="{ 'animation-name': 'bounceInUp','animation-duration': '1.4s'}">           
                <div class="icon"><font-awesome-icon :icon="['far', 'list-alt']" size="2x"></font-awesome-icon></div>
                <h4 class="title"><a href="">Digital Solutions</a></h4>
                <p class="description">We at Reveation Labs provide you with the best of Digital Solutions.

         Be it any technology out team makes sure you  get the best service  </p>
            </b-col>
            <b-col lg="4" md="6" class="box" v-wow="{ 'animation-name': 'bounceInUp','animation-duration': '1.4s'}">     
                <div class="icon"><font-awesome-icon :icon="['far', 'list-alt']" size="2x"></font-awesome-icon></div>
                <h4 class="title"><a href="">Mobility</a></h4>
                <p class="description">We love developing Mobile Applications and our team of expertise has a special affinity to program next generation of Mobile Applications beacause we believe this is where the future is!</p>
            </b-col>
           <b-col lg="4" md="6" class="box" v-wow="{ 'animation-name': 'bounceInUp','animation-duration': '1.4s'}">     
            <div class="icon"><font-awesome-icon :icon="['far', 'list-alt']" size="2x"></font-awesome-icon></div>
            <h4 class="title"><a href="">Cloud Based Solutions</a></h4>
            <p class="description">As the world move towards cloud based solutions. Reveation Labs has a dedicated team which makes the perfect use of cloud based solutions</p>
           </b-col>
           <b-col lg="4" md="6" class="box" v-wow="{ 'animation-name': 'bounceInUp', 'animation-delay': '0.1s', 'animation-duration': '1.4s'}">     
            <div class="icon"><font-awesome-icon :icon="['far', 'list-alt']" size="2x"></font-awesome-icon></div>
            <h4 class="title"><a href="">Blockchain</a></h4>
            <p class="description">Blockchain might sound a new age term. But the highly passionate engineers at Reveation labs have been dealing with Blockchain since years and they make sure to provide you will all tehe guidance to understand the in-depth of this technology</p>
           </b-col>
           <b-col lg="4" md="6" class="box" v-wow="{ 'animation-name': 'bounceInUp', 'animation-delay': '0.1s', 'animation-duration': '1.4s'}">     
            <div class="icon"><font-awesome-icon :icon="['far', 'list-alt']" size="2x"></font-awesome-icon></div>
            <h4 class="title"><a href="">Data Science</a></h4>
            <p class="description">We at reveations labs love to deal with algorithms,maths, statistica with a flare of Programming</p>
           </b-col>
          <b-col lg="4" md="6" class="box" v-wow="{ 'animation-name': 'bounceInUp', 'animation-delay': '0.1s', 'animation-duration': '1.4s'}">     
            <div class="icon"><font-awesome-icon :icon="['far', 'list-alt']" size="2x"></font-awesome-icon></div>
            <h4 class="title"><a href="">PLAY </a></h4>
            <p class="description">Reveation Labs deals with new and exciting frameworks such as PLAY providing you with all the latest trendy solutions </p>
           </b-col>

        </b-row>

      </b-container>
    </section>
</template>

<script>
export default {
}
</script>

<style>
.rl-services {
  background: #fff;
  background-size: cover;
  padding: 60px 0 40px 0;
}

.rl-services .box {
  margin-bottom: 30px;
}

.rl-services .icon {
  float: left;
}

.rl-services .icon path {
  color: #18d26e;
  font-size: 36px;
  line-height: 1;
  transition: 0.5s;
}

.rl-services .title {
  margin-left: 60px;
  font-weight: 700;
  margin-bottom: 15px;
  font-size: 18px;
}

.rl-services .title a {
  color: #111;
}

.rl-services .box:hover .title a {
  color: #18d26e;
}

.rl-services .description {
  font-size: 14px;
  margin-left: 60px;
  line-height: 24px;
  margin-bottom: 0;
}
</style>
