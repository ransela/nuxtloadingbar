<script setup>
const pages = ['/', '/hello', '/world', '/vue'];
</script>

<template>
  <div>
    <NuxtLoadingBar :duration="1000" />
    <ul>
      <li v-for="page of pages">
        <NuxtLink :to="page">{{ page }}</NuxtLink>
      </li>
    </ul>
    <NuxtPage />
  </div>
</template>
