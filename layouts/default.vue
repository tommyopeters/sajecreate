<template>
  <div class="wrapper">
    <div class="particles-wrapper">
      <vue-particles
        color="#000000"
        :particleOpacity="0.7"
        :particlesNumber="120"
        shapeType="circle"
        :particleSize="2"
        linesColor="#dedede"
        :linesWidth="1"
        :lineLinked="true"
        :lineOpacity="0.4"
        :linesDistance="150"
        :moveSpeed="3"
        :hoverEffect="true"
        hoverMode="repulse"
        :clickEffect="true"
        clickMode="push"
      ></vue-particles>
    </div>
    <div class="inner-wrapper">
      <TheHeader />
      <Nuxt />
      <TheFooter />
    </div>
  </div>
</template>

<script>
// https://vue-particles.netlify.app/?ref=madewithvuejs.com
export default {
  mounted() {
    $("#particles-js").height($(".inner-wrapper").height());
  },
};
</script>

<style></style>
