<template>
  <div id="game-scene" :class="{'scene in ':show,'scene out' :!show}">

  </div>
</template>

<script>
  import Constant from './constant'
  export default {
    data () {
      return {
        show: false
      }
    },
    mounted () {
      Constant.Event.$on(Constant.MSG_START_SCENE,
        function () {
          this.show = true
        }.bind(this))
    }
  }
</script>

<style scoped>
</style>
