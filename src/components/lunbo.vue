<template>
     <swiper :options="swiperOption" ref="mySwiper">
    <!-- slides -->
    <swiper-slide><img src="https://dimg04.c-ctrip.com/images/70030y000000m2zuu09AA_1920_340_17.jpg" alt=""></swiper-slide>
    <swiper-slide><img src="https://dimg04.c-ctrip.com/images/700h0z000000nmgjq3189_1920_340_17.jpg" alt=""></swiper-slide>
    <swiper-slide><img src="https://dimg04.c-ctrip.com/images/700q0z000000ndznk42A4_1920_340_17.jpg" alt=""></swiper-slide>
    <swiper-slide><img src="https://dimg04.c-ctrip.com/images/700710000000on3xv48A0_1920_340_17.jpg" alt=""></swiper-slide>


    <!-- Optional controls -->
    <div class="swiper-pagination"  slot="pagination"></div>
    <!-- <div class="swiper-button-prev" slot="button-prev"></div>
    <div class="swiper-button-next" slot="button-next"></div> -->
  </swiper>
</template>
<script>
  export default {
    name: 'carrousel',
    data() {
      return {
        swiperOption: {
        pagination: '.swiper-pagination',
        loop: true,
        speed:1400,
        autoplay:2400,
        preventClicks:false,
        autoplayDisableOnInteraction : false,
        prevButton:'.swiper-button-prev',
        nextButton:'.swiper-button-next',
        autoHeight:true// some swiper options/callbacks
          // 所有的参数同 swiper 官方 api 参数
          // ...
        }
      }
    }

  }

</script>
<style lang="stylus" scoped>
.wrapper >>> .swiper-pagination-bullet-active
    background #fff


  img
    width 100%
    height:2.5rem
</style>
