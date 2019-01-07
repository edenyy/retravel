<template>
  <div class="shouye">
   <iheader></iheader>
   <lunbo></lunbo>
  </div>
</template>

<script>
import iheader from '@/components/header'
import lunbo from '@/components/lunbo'
export default {
  name: 'home',
  components:{
    iheader,
    lunbo
  },
  data () {
    return {
      msg: ''
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang='stylus' scoped>

</style>
