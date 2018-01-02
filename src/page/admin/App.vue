<template>
  <div id="app">

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

table01.methods.init(666);

export default {
  name: 'app',
  components: {
    HelloWorld,slider_ivew_01,table01
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

#slider{

  width: 10%;

}
</style>
