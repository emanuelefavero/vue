<script setup lang="ts">
const fruit = 'mango'
</script>

<template>
  <div>
    <h3>v-else-if</h3>
    <h4 v-if="fruit === 'mango'">Mango</h4>
    <h4 v-else-if="fruit === 'orange'">Orange</h4>
    <h4 v-else>Fruit</h4>
  </div>
</template>
