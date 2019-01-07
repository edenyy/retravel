<template>
    <div class="index">
        <span class="left"> 《 </span>
        <div class="input"></div>
        <div class="right" @click='citychoose'>上海&nbsp;<i class="iconfont icon-xiala"></i></div>
    </div>
</template>
<script>
export default {
name:'header',
methods:{
    citychoose(){
        this.$router.push('/city')
    }
}
}
</script>
<style lang='stylus'>
.index
    height 1rem
    background #cc3399
    display flex
    align-items center
    justify-content space-between
    .left
        flex 1
        margin-left -0.2rem
        color #ffffff
        text-align center
        font-size .4rem
        line-height .4rem
    .input
        border 1px solid #fff
        height 70%
        background #fff
        flex 4
    .right
        height 40%
        text-align center
        flex 1.5
        color #fff
        line-height .4rem
        font-size .4rem
</style>
