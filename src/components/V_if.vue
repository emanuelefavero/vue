<script setup lang="ts">
const showDiv1 = true
const showDiv2 = false
</script>

<template>
  <div>
    <h3>v-if</h3>
    <div v-if="showDiv1">div 1</div>
    <div v-if="showDiv2">div 2</div>
  </div>
</template>
