<template>
  <div id="app">
    <Card />
  </div>
</template>

<script>
import Card from '@/components/Card.vue'

export default {
  name: 'App',
  components: {
    Card
  }
}
</script>

<style lang="scss">
  #app {
    font: {
      family: 'Open Sans', sans-serif;
      weight: 600;
    }
    background-color: #e5e5e5;
  }
</style>
