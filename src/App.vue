<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <test/>
    <LandingBanner/>
    <GameRoom msg="Welcome to Your Vue.js App"/>
    <!-- <Footer></Footer> -->
  </div>
</template>

<script>
import GameRoom from './components/GameRoom.vue'
import LandingBanner from './components/LandingBanner.vue'
import test from './components/test.vue'

export default {
  name: 'app',
  components: {
    LandingBanner,
    GameRoom,
    test
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
