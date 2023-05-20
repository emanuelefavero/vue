<script setup lang="ts">
import { ref } from 'vue'

const show = ref(true)
</script>

<template>
  <div>
    <!-- NOTE: v-show only changes the visibility -->
    <!-- it is faster than v-if -->
    <!-- use it when changing the visibility of an object -->
    <h4 v-show="show">This element can be shown or hidden</h4>
  </div>
</template>
