<template>
  <ul class="list">
    <li class="item" v-for="(item, key) of letter" :key="key">{{key}}</li>
  </ul>
</template>

<script>
export default {
  name: 'CityAlphabet',
  props: {
    letter: Object
  }
}
</script>

<style lang="stylus" scoped>
  @import '~styles/varibles.styl'
  .list
    /*上下居中*/
    display: flex
    flex-direction: column
    justify-content: center
    /*上下居中*/
    position: absolute
    top: 1.58rem
    right: 0
    bottom: 0
    width: .44rem
    /*水平居中*/
    .item
      line-height: .4rem
      text-align: center
      color: $bgColor
    /*水平居中*/
</style>
