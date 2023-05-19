<script setup lang="ts">
import { ref } from 'vue'

const show = ref(true)
</script>

<template>
  <div>
    <button @click="show = !show">{{ show ? 'hide' : 'show' }}</button>
    <span v-if="show">Conditional Rendering</span>
  </div>
</template>
