<template>
  <div>
    <h1>Color Index page</h1>
    <ul>
      <li v-for="color in colors" :key="color">
        <NuxtLink
          :to="`/color/${color}`"
          class="inline-block px-2 p-1 no-underline font-bold text-white bg-red/80 rounded"
          >{{ color }}</NuxtLink
        >
      </li>
    </ul>
  </div>
</template>

<script setup lang="ts">
const colors = ['purple', 'bule', 'yellow']
</script>
