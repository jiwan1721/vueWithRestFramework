<template>
<div id="app">
 <Print-Values :greeting="hello"></Print-Values>
</div>
</template>

<script>
import PrintValues from './components/PrintValues'


export default {
  name: 'app',
  components: {
    PrintValues
},

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
