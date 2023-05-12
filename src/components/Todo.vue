<script setup lang="ts">
import { ref } from 'vue'

const todos = ref<string[]>(['sleep', 'eat', 'code'])
const newTodo = ref('')
</script>

<template>
  <h1>Todo</h1>

  <input type="text" v-model="newTodo" />
  <button type="button" @click="() => todos.push(newTodo)">Add</button>

  <p>
    {{ todos.length === 0 ? 'No todos yet' : '' }}
  </p>

  <ol>
    <li v-for="(todo, index) in todos">
      {{ todo }}
      <button type="button" @click="() => todos.splice(index, 1)">x</button>
    </li>
  </ol>
</template>
