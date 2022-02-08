<template>
  <div class="hot" >
    <div class="swiper-container">
      <div class="swiper-wrapper">
        <div class="swiper-slide"><img src="../imgs/rowing/s1.png" alt="" width="100%"></div>
        <div class="swiper-slide"><img src="../imgs/rowing/s2.png" alt="" width="100%"></div>
        <div class="swiper-slide"><img src="../imgs/rowing/s3.png" alt="" width="100%"></div>
        <div class="swiper-slide"><img src="../imgs/rowing/s4.png" alt="" width="100%"></div>
        <div class="swiper-slide"><img src="../imgs/rowing/s5.png" alt="" width="100%"></div>
        <div class="swiper-slide"><img src="../imgs/rowing/s6.png" alt="" width="100%"></div>
        <div class="swiper-slide"><img src="../imgs/rowing/s7.png" alt="" width="100%"></div>
      </div>
      <!-- 如果需要分页器 -->
      <div className="swiper-pagination"></div>
    </div>
    <!--    &lt;!&ndash;2.中间导航&ndash;&gt;-->
    <!--    <hot-nav/>-->
    <!--    &lt;!&ndash;3.广告位&ndash;&gt;-->
    <!--    <div class="hot-ad">-->
    <!--      <img src="./../../imgs/hot_ad/home_ad.gif" alt="" width="100%">-->
    <!--    </div>-->
    <!--    &lt;!&ndash;4.商品的列表&ndash;&gt;-->
    <!--    <hot-shop-list />-->

  </div>
</template>

<script>
import Swiper from 'swiper'
import 'swiper/dist/css/swiper.min.css'

// import HotNav from './HotNav'
// import HotShopList from './HotShopList'

export default {
  name: "Hot",
  // components:{
  //   HotNav,
  //   HotShopList
  // },
  mounted() {
    // 创建swiper的实例
    new Swiper('.swiper-container', {
      autoplay: true,//等同于以下设置
      loop: true,
      // 如果需要分页器
      pagination: {
        el: '.swiper-pagination',
        observeParents:true,
        observer:true,
      }
    })
  }
}
</script>

<style scoped lang="stylus" ref="stylesheet/stylus">
.hot
  width 100%
  height 100%
  padding-top 46px
  background #F5F5F5

//.hot-ad
//  background-color #fff
//  margin 8px 0
//  padding 5px
</style>
