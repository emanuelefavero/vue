<script setup lang="ts">
import { ref } from 'vue'

defineProps<{ greet: string }>()

const count = ref(1)
</script>

<template>
  <h1 class="title">{{ greet }}</h1>

  <h2>{{ count }}</h2>

  <button type="button" @click="() => count--">-</button>
  <button type="button" @click="() => count++">+</button>
</template>

<style scoped>
.title {
  color: magenta;
}

h2 {
  color: limegreen;
}
</style>
