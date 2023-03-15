<template>
  <div>
    <Header />
    <Hero />
    <WhyUs />
    <Countdown />
    <Speakers />
    <Program />
    <Map />
    <Location />
  </div>
</template>

<!-- ************************************************************************** -->

<script>
import Header from './components/Header.vue';
import Hero from './components/Hero.vue';
import WhyUs from './components/WhyUs.vue'
import Countdown from './components/Countdown.vue';
import Speakers from './components/Speakers.vue';
import Program from './components/Program.vue';
import Map from './components/Map.vue';
import Location from './components/Location.vue';

  export default {
    components:{
      Header,
      Hero,
      WhyUs,
      Countdown,
      Speakers,
      Program,
      Map,
      Location,
    }
  }
</script>

<!-- ************************************************************************** -->

<style lang="scss" scoped>


</style>