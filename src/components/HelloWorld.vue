<script setup lang="ts">
import { ref } from 'vue'

defineProps<{ msg: string }>()

const count = ref(1)
</script>

<template>
  <h1>{{ msg }}</h1>

  <h2>{{ count }}</h2>
  <button
    type="button"
    @click="
      () => {
        if (count > 0) {
          count--
        }
      }
    "
  >
    -
  </button>
  <button type="button" @click="() => count++">+</button>
</template>
