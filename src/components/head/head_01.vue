<template>


  <div>
    <Row>
      <Col span="12">col-12</Col>
      <Col span="12">col-12</Col>
    </Row>

    <Button type="primary" id="ok" v-on:click="move">Primary</Button>

  </div>


</template>

<script>


  import snabbt from 'snabbt.js'

  export default {
    name: "head_01",

    methods: {

      move: function () {

        var container = document.getElementById('ok');
        snabbt(container, {
          position: [200, 20, 0],
          rotation: [0, 0, 1*Math.PI],
          easing: 'spring',
          springConstant: 0.5,
          springDeceleration: 0.5
        }).snabbt({
          rotation:[0,0,0],
          complete:function () {
            console.log(this)
          }
        })


      }
    }
  }
</script>

<style scoped>

</style>
