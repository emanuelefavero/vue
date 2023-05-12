<script setup lang="ts">
const customClass = 'custom-class'
</script>

<template>
  <div>
    <!-- TIP: Double mustache can't be used to pass data to html attributes -->
    <!-- NOTE: You can't do this!!! class={{customClass}} -->
    <!-- you need to use v-bind:class, v-bind:id... -->
    <!-- the shorthand is :class, :id -->
    <h3 :class="customClass">Html Attributes State Variables</h3>
  </div>
</template>

<style scoped>
.custom-class {
  color: slateblue;
}
</style>
