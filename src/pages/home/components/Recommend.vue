<template>
  <div>
    <div class="title">热销推荐</div>
    <ul>
      <li class="item border-bottom" v-for="item in recommendList" :key="item.id">
          <img :src="item.imgUrl" class="item-img">
        <div class="item-info">
          <p class="item-title">{{item.title}}</p>
          <p class="item-desc">{{item.desc}}</p>
          <button class="item-button">查看详情</button>
        </div>
      </li>
    </ul>
  </div>
</template>
<script>
export default {
  name: 'HomeRecommend',
  data () {
    return {
      recommendList: [{
        id: '0001',
        title: '大连圣亚海洋世界',
        desc: '浪漫大连首站,浪漫的海洋主题公园',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/201404/23/04b92c99462687fa1ba45c1b5ba4ad77.jpg_150x150_2c4b6f2f.jpg'
      },
      {
        id: '0002',
        title: '大连圣亚海洋世界',
        desc: '浪漫大连首站,浪漫的海洋主题公园',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/201404/23/04b92c99462687fa1ba45c1b5ba4ad77.jpg_150x150_2c4b6f2f.jpg'
      },
      {
        id: '0003',
        title: '大连圣亚海洋世界',
        desc: '浪漫大连首站,浪漫的海洋主题公园',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/201404/23/04b92c99462687fa1ba45c1b5ba4ad77.jpg_150x150_2c4b6f2f.jpg'
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
  .item
    display : flex
    height : 1.9rem
    overflow : hidden
    .item-img
      width : 1.7rem
      height : 1.7rem
      padding : .1rem
    .item-info
      flex : 1
      padding : .1rem
      min-width : 0
      .item-title
        line-height : .54rem
        font-size : .32rem
        ellipis()
      .item-desc
        line-height : .4rem
        color : #ccc
        ellipis()
      .item-button
        line-height : .5rem
        margin-top : .16rem
        background : #ff9300
        padding : 0 .2rem
        border-radius : .06rem
        margin-top : .2rem
        color : #fff
</style>
