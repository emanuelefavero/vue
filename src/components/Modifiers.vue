<script setup lang="ts">
function submit() {
  console.log('submit clicked')
}
</script>

<template>
  <div>
    <form>
      <h3>Modifiers</h3>
      <input type="text" />

      <!-- .prevent is a modifier that calls event.preventDefault() -->
      <!-- TIP: There are other modifiers in vue -->
      <button @click.prevent="submit">Submit</button>
    </form>
  </div>
</template>
