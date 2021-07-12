<template>
  <div id="app">
    <h1>Todos</h1>
    <h3>Completed:{{ $store.getters.completedTodos}}</h3>
    <h3>Pending:</h3>
    <TodosList/>
    <Todoform/>
  </div>
</template>

<script>
import TodosList from './components/TodosList.vue'
import Todoform from './components/Todoform.vue'

export default {
  name: 'App',
  components: {
    TodosList,
    Todoform
  }
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
