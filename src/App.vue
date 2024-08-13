<template>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Alata&family=Manrope:wght@200..800&family=Plus+Jakarta+Sans:ital,wght@0,200..800;1,200..800&family=Space+Mono:ital,wght@0,400;0,700;1,400;1,700&display=swap" rel="stylesheet">
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Alata&family=Josefin+Sans:ital,wght@0,100..700;1,100..700&family=Manrope:wght@200..800&family=Plus+Jakarta+Sans:ital,wght@0,200..800;1,200..800&family=Space+Mono:ital,wght@0,400;0,700;1,400;1,700&display=swap" rel="stylesheet">
  <div class="Header">
    <NavMain />
      <MainHeader />
  </div>
  <div class="top">
    <TopSection />
  </div>
  <div class="bottom">
    <SectionBottom />
    <BottomNav />
  </div>
  
</template>

<script>
import BottomNav from './components/BottomNav.vue';
import MainHeader from './components/MainHeader.vue';
import NavMain from './components/NavMain.vue';
import SectionBottom from './components/SectionBottom.vue';
import TopSection from './components/TopSection.vue';

export default {
  name: 'App',
  components: {
    NavMain,
    MainHeader,
    TopSection,
    SectionBottom,
    BottomNav
  }
}
</script>

<style>
@import url('./assets/index.css');
</style>
