<template>
<div id="app">
  <TasksVue></TasksVue>
</div>
</template>

<script>
import TasksVue from './components/TasksVue.vue'

export default {
  name: 'App',
  components: {
    TasksVue,
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
