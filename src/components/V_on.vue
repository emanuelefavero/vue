<script setup lang="ts">
import { ref } from 'vue'
const color = ref('red')

// TIP: we use .value to access the value of a ref
function changeColor() {
  color.value = color.value === 'red' ? 'cyan' : 'red'
}
</script>

<template>
  <div>
    <h2 :style="{ color: color }">v-on</h2>
    <!-- v-on is the directive for v-on:click, v-on:change -->
    <!-- the shorthand is @ -->
    <button type="button" @click="changeColor">Change Color</button>
  </div>
</template>
