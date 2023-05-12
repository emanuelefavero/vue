<script setup lang="ts">
import { ref } from 'vue'

// TIP: ref is similar of useState in React
const count = ref(1)

// TIP: To access the value of a ref, we use .value (like .current in React)
function reset() {
  count.value = 1
}
</script>

<template>
  <div>
    <h3>ref</h3>
    <h4>{{ count }}</h4>
    <button @click="count++">Add</button>
    <button @click="reset">Reset</button>

    <!-- TIP: When using the ref variable here we don't need .value -->
    <button @click="count = 1">Reset 2</button>
  </div>
</template>
