<template>
  <div>
    <div flex="~ gap-3" items-center mb-4>
      <p>Counter: {{ counter }}</p>
      <button @click="counter++" w-8 h-8 rounded bg="green">+</button>
      <button @click="counter--" w-8 h-8 rounded bg="red">-</button>
    </div>
      <NuxtLink
        :to="`/counter/${counter}`"
        class="inline-block px-2 p-1 no-underline font-bold text-white bg-red/80 rounded"
        >Open /counter/{{ counter }}</NuxtLink
      >
    <p>Bellow is a nested page</p>
    <NuxtPage />
  </div>
</template>

<script setup lang="ts">
const counter = useCounter()
</script>
