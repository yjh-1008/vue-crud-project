<template>
  <div id="app">
    <TextArea/>
    <router-view/>
  </div>
</template>

<script>
import TextArea from './components/TextArea.vue'
export default {
  name: 'App',
  components: {
    'TextArea': TextArea
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
