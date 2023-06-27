<template>
  <AppHeader/>
  <TopCarousel/>
  <AppMain/>
  <BottomCarousel/>
  <AppFooter/>
</template>
<script>
import AppHeader from './components/AppHeader.vue';
import TopCarousel from './components/TopCarousel.vue';
import AppMain from './components/AppMain.vue';
import BottomCarousel from './components/FooterContents/BottomCarousel.vue';
import AppFooter from './components/AppFooter.vue';
export default {
    name:"App",
    components:{
      AppHeader,
      TopCarousel,
      AppMain,
      BottomCarousel,
      AppFooter
    }
}
</script>
<style lang="scss">
@import './styles/general.scss'
  
</style>