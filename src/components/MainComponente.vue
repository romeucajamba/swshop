<script setup lang="ts">
import { RouterView } from 'vue-router'
defineProps<{
  msg: string
}>()
</script>

<template>
  <main>
    <h1 class="green">{{ msg }}</h1>
    <h3>
      You’ve successfully created a project with
      
    </h3>
    
  </main>
</template>

<style scoped>
@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
}
</style>
