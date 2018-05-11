<template>
  <div>
    <div class="title">周末去哪</div>
    <ul>
      <li class="item border-bottom" v-for="item in recommendList" :key="item.id">
        <div class="item-img-wrapper">
          <img :src="item.imgUrl" class="item-img">
        </div>
        <div class="item-info">
          <p class="item-title">{{item.title}}</p>
          <p class="item-desc">{{item.desc}}</p>
        </div>
      </li>
    </ul>
  </div>
</template>
<script>
export default {
  name: 'HomeWeekend',
  data () {
    return {
      recommendList: [{
        id: '0001',
        title: '大连圣亚海洋世界',
        desc: '浪漫大连首站,浪漫的海洋主题公园',
        imgUrl: 'http://img1.qunarzz.com/sight/source/1505/7f/fa4eb0ca72409d.jpg_r_640x214_2f2a860e.jpg'
      },
      {
        id: '0002',
        title: '大连圣亚海洋世界',
        desc: '浪漫大连首站,浪漫的海洋主题公园',
        imgUrl: 'http://img1.qunarzz.com/sight/source/1505/7f/fa4eb0ca72409d.jpg_r_640x214_2f2a860e.jpg'
      },
      {
        id: '0003',
        title: '大连圣亚海洋世界',
        desc: '浪漫大连首站,浪漫的海洋主题公园',
        imgUrl: 'http://img1.qunarzz.com/sight/source/1505/7f/fa4eb0ca72409d.jpg_r_640x214_2f2a860e.jpg'
      }]
    }
  }
}
</script>
<style lang="stylus" scoped>
  @import '~styles/mixins.styl'
  .title
    margin-top : .2rem
    line-height : .8rem
    background : #eee
    text-indent : .2rem
  .item-img-wrapper
    overflow : hidden
    height:0
    padding-bottom : 33.9%
    .item-img
      width : 100%
  .item-info
    padding : .1rem
    .item-title
      line-height : .54rem
      font-size : .32rem
      ellipis()
    .item-desc
      line-height : .4rem
      color : #ccc
      ellipis()
</style>
