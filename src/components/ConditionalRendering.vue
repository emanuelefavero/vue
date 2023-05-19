<script setup lang="ts">
import { ref } from 'vue'

const show = ref(true)

const numbers = ref([3, 3])
const sumIsBiggerThan = (value: number) => {
  const sum = numbers.value.reduce((total: number, num: number) => total + num)
  return sum > value
}
</script>

<template>
  <div>
    <button @click="show = !show">{{ show ? 'hide' : 'show' }}</button>
    <span v-if="show">Conditional Rendering</span>

    <h3 v-if="sumIsBiggerThan(5)">Sum is bigger than 5</h3>
    <h3 v-else-if="sumIsBiggerThan(10)">Sum is bigger than 10</h3>
    <h3 v-else>Sum is smaller than 5</h3>
  </div>
</template>
