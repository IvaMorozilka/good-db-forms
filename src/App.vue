<script setup>
import { RouterView } from 'vue-router'
</script>

<template>
  <header>
    <h1>Это главная страница</h1>
    <h2>Будет хидер, для переключения форм</h2>
  </header>
  <p>Здесь будут формы для заполнения<br>Первая - Гумманитарная помощь.</p>
  <RouterView />
</template>

<style scoped>
</style>
