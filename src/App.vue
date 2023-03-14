<template>
  <div>
    <Header />
    <Hero />
    <WhyUs />
    <Countdown />
  </div>
</template>

<!-- ************************************************************************** -->

<script>
import Header from './components/Header.vue';
import Hero from './components/Hero.vue';
import WhyUs from './components/WhyUs.vue'
import Countdown from './components/Countdown.vue';

  export default {
    components:{
      Header,
      Hero,
      WhyUs,
      Countdown,
    }
  }
</script>

<!-- ************************************************************************** -->

<style lang="scss" scoped>


</style>