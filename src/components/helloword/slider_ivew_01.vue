<template>

  <Slider v-model="value" range></Slider>

</template>

<script>
    export default {
        name: "slider_ivew_01",
        data () {
        return {
          value: [20, 50]
        }
      }
    }
</script>

<style scoped>

</style>
