<template>
  <div>
    <ul>
      <li>
        <TodoItem
          v-for="todo of todos"
          v-bind:todo="todo"
        />
      </li>
    </ul>
  </div>
</template>

<script>
import TodoItem from "@/components/TodoItem"
export default {
  props: ['todos'],
  components: {
    TodoItem
  }
  
}
</script>