<template>
  <div>
    <Header />
    <Hero />
    <WhyUs />
  </div>
</template>

<!-- ************************************************************************** -->

<script>
import Header from './components/Header.vue';
import Hero from './components/Hero.vue';
import WhyUs from './components/WhyUs.vue'

  export default {
    components:{
      Header,
      Hero,
      WhyUs,
    }
  }
</script>

<!-- ************************************************************************** -->

<style lang="scss" scoped>


</style>