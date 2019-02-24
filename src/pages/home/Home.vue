<template>
  <div>
    <home-header></home-header>
    <swiper-header></swiper-header>
    <home-icons></home-icons>
  </div>
</template>

<script>
import HomeHeader from './components/Header'
import SwiperHeader from './components/Swiper'
import HomeIcons from './components/Icons'
export default {
  name: 'Home',
  components: {HomeIcons, SwiperHeader, HomeHeader},
  comments: {
    HomeHeader: HomeHeader,
    SwiperHeader: SwiperHeader,
    HomeIcons: HomeIcons
  }
}
</script>

<style scoped>

</style>
