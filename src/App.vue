<template>
  <div id="app">
    <!--左侧导航-->
    <leftNav></leftNav>
    <div class="main">
       <router-view/>
    </div>
  </div>
</template>

<script>
import leftNav from '@/components/common/leftNav'
export default {
  name: 'App',
  components: {
    leftNav
  }
}
</script>

<style>
html,
body,
#app {
width: 100%;
height: 100%;
padding: 0;
margin: 0;
}
#app {
  font-family: "Microsoft YaHei","MicrosoftJhengHei",'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
.main{
  float:left;
  width:95%;
  background-color: #EFF2F7;
  height:100%;
  overflow: auto;
}
</style>
