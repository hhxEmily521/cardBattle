<template>
  <div >
  <header>
    <div class="row">
      <h1>卡牌游戏</h1>
      <section id="game" class="row">
         <start-scene></start-scene>
        <game-scene></game-scene>
      </section>
    </div>
  </header>
    <section class="how-to-paly">
      <h2>游戏介绍</h2>
      <p>选择任意一张牌然后看点数的pk结果</p>

    </section>
    <footer>
      <p>给我个打赏吧 </p>
      <img id="payme" src="../../static/logo.png">
    </footer>
  </div>
</template>

<script>
   import StartScene from './startscrenecomponet'
   import GameScene from './gamescenecomponet'
   export default {
     components: {
       StartScene,
       GameScene
     }}
</script>

<style scoped>/*//只作用于本页面的HTML或者只作用于子组件代码*/
 #game{
   width: 480px;
   height:600px;
   border-radius: 8px;
   overflow: hidden;
 }
.scene {
  width: 100%;
  height: 100%;
  position: absolute;
  overflow: hidden;
  border-radius: 8px;
  transition: all .3s ease-out;
}
  #payme{
    width: 240px;
    height: 256px;
    margin: 0 auto;
  }
</style>

