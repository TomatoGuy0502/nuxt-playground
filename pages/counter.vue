<template>
  <div>
    <div flex="~ gap-3" items-center mb-4>
      <p>Counter: {{ counter }}</p>
      <button @click="counter++" w-8 h-8 rounded bg="green">+</button>
      <button @click="counter--" w-8 h-8 rounded bg="red">-</button>
    </div>
    <NuxtLink
      :to="`/counter/${counter}`"
      class="bg-red/80 inline-block rounded p-1 px-2 font-bold text-white no-underline"
      >Open /counter/{{ counter }}</NuxtLink
    >
    <p>Bellow is a nested page</p>
    <NuxtPage />
  </div>
</template>

<script setup lang="ts">
const counter = useCounter()
</script>
