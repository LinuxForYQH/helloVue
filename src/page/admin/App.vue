<template>
  <div id="app">

    <div id="head_01">
      <head_01/>
    </div>

    <div id="slider">
      <slider_ivew_01/>
    </div>

    <div id="table">
      <table01/>
    </div>

  </div>
</template>

<script>
import HelloWorld from '../../components/helloword/HelloWorld'
import slider_ivew_01 from '../../components/helloword/slider_ivew_01'
import table01 from '../../components/datatable/table01'
import head_01 from '../../components/head/head_01'

table01.methods.init();

export default {
  name: 'app',
  components: {
    HelloWorld,slider_ivew_01,table01,head_01
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}

#slider{
  width: 10%;
}
</style>
