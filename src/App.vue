<template>
  <GamePanel msg="puzzle game"/>
</template>

<script>
import GamePanel from "@/components/GamePanel";

export default {
  name: 'App',
  components: {
    GamePanel
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
