<template>
  <div>
    <header flex="~ gap-4" p-2 px-4 border="b-2 gray">
      <NuxtLink to="/" p-2 bg="gray hover:gray/80" rounded text-white font-bold> Home </NuxtLink>
      <NuxtLink to="/counter" p-2 bg="gray hover:gray/80" rounded text-white font-bold> Counter </NuxtLink>
      <NuxtLink to="/color" p-2 bg="gray hover:gray/80" rounded text-white font-bold> Color </NuxtLink>
    </header>
    <main p-2>
      <slot />
    </main>
  </div>
</template>

<script setup lang="ts"></script>
