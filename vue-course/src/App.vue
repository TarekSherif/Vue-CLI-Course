<template>
  <div id="app">
 
    <BindingExamples/>
  </div>
</template>

<script>
 
import BindingExamples from './components/BindingExamples.vue'


export default {
  name: 'app',
  components: {
   
    BindingExamples
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
