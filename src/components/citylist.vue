<template>
    <div class="list" ref='wrap'>
        <div>
        <div class="header">您的位置</div>
        <div class="content"><div class="button">北京</div></div>
        <div class="header">热门城市</div>
        <div class="content hot">
        <div class="button" :class="{active:istrue}" @click='xz'>北京</div>
        <div class="button">上海</div>
        <div class="button">南京</div>
        <div class="button">武汉</div>
        <div class="button">杭州</div><div class="button">昆明</div><div class="button">深圳</div>

        </div>
         <div class="header">A</div>
        <div class="content"><li>阿富汗</li>
        <li>阿富汗</li>
        <li>阿富汗</li>
        <li>阿富汗</li>
        <li>阿富汗</li>
        <li>阿富汗</li>
        <li>阿富汗</li>
        <li>阿富汗</li></div>

         <div class="header">B</div>
        <div class="content"><li>阿富汗</li>
        <li>阿富汗</li>
        <li>阿富汗</li>
        <li>阿富汗</li>
        <li>阿富汗</li>
        <li>阿富汗</li>
        <li>阿富汗</li>
        <li>阿富汗</li></div>
        </div>
    </div>

</template>
<script>
import BScroll from 'better-scroll'
export default {
   name:'list',
   data(){
       return{
        istrue:false
       }
   },
   methods:{
       xz(){
           this.istrue=true
           console.log('true')
       }
   },
   mounted(){
       let bs=new BScroll(this.$refs.wrap)
   }
}
</script>
<style lang="stylus" scoped>
.list
    height 13.5rem
    overflow hidden


    .header
        background #eee
        height:.5rem
        padding .2rem 0 0 .2rem
        font-size .3rem
        font-weight bold
    .hot
        display flex
        flex-wrap wrap
    .content
        background #fff
    .content li
        font-size .26rem
        list-style none
        height .6rem
        padding .1rem 0 0 .2rem
    .content  .active
            border 0.02rem solid blue
        .button
            padding-top 0.09rem
            width 2rem
            height .4rem
            margin .2rem 0 .2rem .2rem
            text-align center
            border-radius .1rem
            border 0.02rem solid #eee
</style>
