<template>
  <div>
    <header>
      <NuxtLink to="/"> Home </NuxtLink>
      <NuxtLink to="/counter"> Counter </NuxtLink>
      <NuxtLink to="/color"> Color </NuxtLink>
    </header>
    <main>
      <slot />
    </main>
  </div>
</template>

<script setup lang="ts"></script>
