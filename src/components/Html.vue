<script setup lang="ts">
const html = '<h3>Hello, Html</h3>'
</script>

<template>
  <!-- {{  }} this is called the mustache syntax -->
  <!-- this type of data binding interpret data as plain text -->
  {{ html }}

  <!-- if you need to pass html, use the v-html directive -->
  <div v-html="html"></div>
</template>

<style>
h3 {
  color: lime;
}
</style>
