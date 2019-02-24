<template>
  <div class="wrapper">
    <swiper :options="swiperOption">
      <swiper-slide v-for="item of swiperList" :key="item.id">
        <img class="swiper-img" :src="item.imgUrl"/>
      </swiper-slide>
      <div class="swiper-pagination"  slot="pagination"></div>
    </swiper>
  </div>
</template>

<script>
export default {
  name: 'SwiperHeader',
  data: function () {
    return {
      swiperOption: {
        pagination: '.swiper-pagination',
        loop: true
      },
      swiperList: [
        {
          id: '001',
          imgUrl: 'http://mp-piao-admincp.qunarzz.com/mp_piao_admin_mp_piao_admin/admin/20191/a' +
            '211765c0bb579b18c6e7d6d75997a48.jpg_750x200_b6921fa6.jpg'
        },
        {
          id: '002',
          imgUrl: 'http://mp-piao-admincp.qunarzz.com/mp_piao_admin_mp_piao_admin/admin/20191/1' +
            '59c25f6c0e024acf3f65d70241846e6.jpg_750x200_b1fe75d5.jpg'
        },
        {
          id: '003',
          imgUrl: 'http://mp-piao-admincp.qunarzz.com/mp_piao_admin_mp_piao_admin/admin/20192/c' +
            '64e6f7308f67f0862adb64b9d9fcff0.jpg_750x200_37c4c320.jpg'
        }
      ]
    }
  }
}
</script>

<style scoped lang="stylus">
  // <!-- 穿透 -->
  .wrapper >>> .swiper-pagination-bullet-active
    background: #fff
  .wrapper
    overflow: hidden
    width: 100%
    height: 0
    padding-bottom: 25%
    background: #eee
    .swiper-img
      width: 100%
</style>
