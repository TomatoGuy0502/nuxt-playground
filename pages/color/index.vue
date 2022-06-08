<template>
  <div>
    <h1>Color Index page</h1>
    <ul>
      <li v-for="color in colors" :key="color">
        <NuxtLink :to="`/color/${color}`">{{ color }}</NuxtLink>
      </li>
    </ul>
  </div>
</template>

<script setup lang="ts">
const colors = ['purple', 'bule', 'yellow']
</script>
