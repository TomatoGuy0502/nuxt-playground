<template>
  <div>
    <div>
      Counter: {{ counter }}
      <button @click="counter++">+</button>
      <button @click="counter--">-</button>
      <NuxtLink :to="`/counter/${counter}`">Open /counter/{{ counter }}</NuxtLink>
    </div>
    <p>Bellow is a nested page</p>
    <NuxtPage />
  </div>
</template>

<script setup lang="ts">
const counter = useCounter()
</script>
