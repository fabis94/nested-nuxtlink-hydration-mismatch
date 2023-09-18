<template>
    <div class="index">
        <NuxtLink to="/other" class="card">
      <span>NuxtLink top text</span>
      <NuxtLink @click.stop.prevent="onNestedClick">Nested nuxt link</NuxtLink>
      <span>NuxtLink bottom text</span>
    </NuxtLink>
    </div>
  </template>
  <script setup lang="ts">
  const onNestedClick = () => {
    console.log("nested nuxtlink clicked")
  }
  </script>
  <style>
  .card {
    display: flex;
    flex-direction: column;
    border: 1px solid black;
    padding: 4px;
    margin-left: auto;
    margin-right: auto;
    width: 300px;
  }
  </style>
  