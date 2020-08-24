<template>
  <div id="app">
    <h1>Todo application</h1>
    <hr>
    <TodoList 
      v-bind:todos="doings"
    />
  </div>
</template>

<script>
import TodoList from "@/components/TodoList"
export default {
  name: 'App',
  components: {
    TodoList
  },
  data() {
    return {
      doings: [
        {id: 1, title: "Купить хлеб", completed: false},
        {id: 2, title: "Купить масло", completed: false},
        {id: 3, title: "Купить индейку", completed: false}
      ]
    }
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
