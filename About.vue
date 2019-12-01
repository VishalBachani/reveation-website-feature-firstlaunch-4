<template>
  <section id="about" class="rl-about">
      <b-container>

        <header class="section-header fadeInUp"  v-wow="{ 'animation-name': 'fadeInUp' }">
          <h3>About Us</h3>
          <p>  The Dynamics of the Technology is changing at a rapid pace. The new innovation comes with its own set of complex problems.We at Reveation Labs are commited to not only solve your complex problems but be your ever reliable tech partner</p>
        </header>

        <b-row class="about-cols">
          <b-col md="4" class="fadeInUp" v-wow="{ 'animation-name': 'fadeInUp','animation-delay': '0.2s'}">
            <div class="about-col">
              <div class="img">
                <b-img-lazy alt="" :src="require('@/assets/images/about/about-mission.jpg')" fluid></b-img-lazy>                
                <div class="icon"><font-awesome-icon :icon="['fas', 'tachometer-alt']" size="2x"  :style="{ color: 'white' }"></font-awesome-icon></div>
              </div>
              <h2 class="title"><a href="#">Our Mission</a></h2>
              <p>
                The mission of Reveation Lab is to stand beside your organisation to aid them in providing the world class and next generation of Digital Solutions which in helps grow your business exponentitally
              </p>
            </div>
          </b-col>

          <b-col md="4" class="fadeInUp" v-wow="{ 'animation-name': 'fadeInUp','animation-delay': '0.4s'}">
            <div class="about-col">
              <div class="img">
                <b-img-lazy alt="" :src="require('@/assets/images/about/about-plan.jpg')" fluid></b-img-lazy>
                <div class="icon"><font-awesome-icon :icon="['far', 'list-alt']" size="2x"  :style="{ color: 'white' }"></font-awesome-icon></div>
              </div>
              <h2 class="title"><a href="#">Our Plan</a></h2>
              <p>
               We belive in the strategy of innovating, the team at Reveation Labs never calls it a day and keeps exploring untill we find the perfect tailor made soltuions for all your needs
              </p>
            </div>
          </b-col>

          <b-col md="4" class="fadeInUp" v-wow="{ 'animation-name': 'fadeInUp','animation-delay': '0.6s'}">
            <div class="about-col">
              <div class="img">
                <b-img-lazy alt="" :src="require('@/assets/images/about/about-vision.jpg')" fluid></b-img-lazy>
                <div class="icon"><font-awesome-icon :icon="['far', 'eye']" size="2x"  :style="{ color: 'white' }"></font-awesome-icon></div>
              </div>
              <h2 class="title"><a href="#">Our Vision</a></h2>
              <p>
                Our Vision is to bring out the most transforming and exciting solution to all your complex business problems
              </p>
            </div>
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

.rl-about {
  background: url("~@/assets/images/about/about-bg.jpg") center top no-repeat fixed;
  background-size: cover;
  padding: 60px 0 40px 0;
  position: relative;
}

.rl-about::before {
  content: '';
  position: absolute;
  left: 0;
  right: 0;
  top: 0;
  bottom: 0;
  background: rgba(255, 255, 255, 0.92);
  z-index: 9;
}

.rl-about .container {
  position: relative;
  z-index: 10;
}

.rl-about .about-col {
  background: #fff;
  border-radius: 0 0 4px 4px;
  box-shadow: 0px 2px 12px rgba(0, 0, 0, 0.08);
  margin-bottom: 20px;
}

.rl-about .about-col .img {
  position: relative;
}

.rl-about .about-col .img img {
  border-radius: 4px 4px 0 0;
}

.rl-about .about-col .icon {
  width: 64px;
  height: 64px;
  padding-top: 8px;
  text-align: center;
  position: absolute;
  background-color: #18d26e;
  border-radius: 50%;
  text-align: center;
  border: 4px solid #fff;
  left: calc( 50% - 32px);
  bottom: -30px;
  transition: 0.3s;
}

.rl-about .about-col i {
  font-size: 36px;
  line-height: 1;
  color: #fff;
  transition: 0.3s;
}

.rl-about .about-col:hover .icon {
  background-color: #fff;
}

.rl-about .about-col:hover svg {
  color: #18d26e !important;
}

.rl-about .about-col h2 {
  color: #000;
  text-align: center;
  font-weight: 700;
  font-size: 20px;
  padding: 0;
  margin: 40px 0 12px 0;
}

.rl-about .about-col h2 a {
  color: #000;
}

.rl-about .about-col h2 a:hover {
  color: #18d26e;
}

.rl-about .about-col p {
  font-size: 14px;
  line-height: 24px;
  color: #333;
  margin-bottom: 0;
  padding: 0 20px 20px 20px;
}
</style>
