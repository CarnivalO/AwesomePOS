
<template>
  <div id="app">
    <!--侧边栏-->
    <leftNav></leftNav>
    <!--主操作-->
    <div class="main">
    <router-view></router-view>
    </div>

  </div>
</template>

<script>
import leftNav from '@/components/common/leftNav'
export default {
  name: 'app',
  components: {
    leftNav
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
}
.main {
  float: left;
  width: 95%;
  background-color: #EFF2F7;
  height: 100%;
  overflow: hidden;
}
</style>
