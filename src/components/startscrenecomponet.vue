<template>
  <div id="start-scene" class="scene">
   <a href="#" id="start-btn" class="button" @click="startBtnClick()"></a>

  </div>
</template>

<script>
  import Constant from './constant'
  export default {
    methods: {
      startBtnClick () {
        Constant.Event.$emit(Constant.MSG_START_SCENE)
      }
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  #start-scene {
    background: url(../../static/logo.png) no-repeat;
  }

  .button {
    position: absolute;
    width: 100%;
    height: 100%;
    top: 0;
    left: 0;

  }

</style>
