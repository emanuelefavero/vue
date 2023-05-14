<script setup lang="ts">
import Hello from './components/Hello.vue'
import Todo from './components/Todo.vue'
import Html from './components/Html.vue'
import HtmlAttributesVariables from './components/HtmlAttributesVariables.vue'
import V_if from './components/V_if.vue'
import V_else_if from './components/V_else_if.vue'
import V_on from './components/V_on.vue'
import Ref from './components/Ref.vue'
import Modifiers from './components/Modifiers.vue'
</script>

<template>
  <Hello greet="Ciao" />
  <Todo />
  <Html />
  <HtmlAttributesVariables />
  <V_if />
  <V_else_if />
  <V_on />
  <Ref />
  <Modifiers />
</template>
