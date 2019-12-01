<template>
  <section id="featured-services" class="rl-featured-services">
    <b-container>
      <b-row>
        <b-col lg="4" class="box">
          <i class="ion-ios-bookmarks-outline"></i>
          <h4 class="title">
            <a href>Commitment</a>
          </h4>
          <p
            class="description"
          >Reveation labs has the next level of commitment which provides you with a smooth sailing </p>
        </b-col>

        <b-col lg="4" class="box box-bg">
          <i class="ion-ios-stopwatch-outline"></i>
          <h4 class="title">
            <a href>Tech Driven</a>
          </h4>
          <p
            class="description"
          >Reveations Labs has the tendency to turn your Business Idea into a Digital Solution</p>
        </b-col>

        <b-col lg="4" class="box">
          <i class="ion-ios-heart-outline"></i>
          <h4 class="title">
            <a href>Satisfication</a>
          </h4>
          <p
            class="description"
          >Our core values lies in providing satisfication to our estemmed clients </p>
        </b-col>
      </b-row>
    </b-container>
  </section>
</template>

<script>
export default {};
</script>

<style>
/* Featured Services Section
--------------------------------*/

.rl-featured-services {
  background: #000;
}

.rl-featured-services .box {
  padding: 30px 20px;
}

.rl-featured-services .box-bg {
  background-image: linear-gradient(
    0deg,
    #000000 0%,
    #242323 50%,
    #000000 100%
  );
}

.rl-featured-services i {
  color: #18d26e;
  font-size: 48px;
  display: inline-block;
  line-height: 1;
}

.rl-featured-services h4 {
  font-weight: 400;
  margin: 15px 0;
  font-size: 18px;
}

.rl-featured-services h4 a {
  color: #fff;
}

.rl-featured-services h4 a:hover {
  color: #18d26e;
}

.rl-featured-services p {
  font-size: 14px;
  line-height: 24px;
  color: #fff;
  margin-bottom: 0;
}
</style>
