<script setup>
import { RouterView } from 'vue-router'
import { Button } from 'primevue';

import JSConfetti from 'js-confetti'

const jsConfetti = new JSConfetti()

</script>

<template>
  <header>
    <h1 class="f">Это главная страница</h1>
    <h2>Будет navbar, для навигации по формам</h2>
  </header>
  <p>Здесь будут формы для заполнения<br>Первая - Гумманитарная помощь.</p>
  <div class="container">
    <Button @click="jsConfetti.addConfetti()">Запустить конфети</Button>
  </div>
  <RouterView />
</template>

<style scoped>
header {
  text-align: center;
}

p {
  padding-top: 100px;
  text-align: center;
  line-height: 2em;
}

.container {
  padding: 20px;
  display: flex !important;
  justify-content: center;
}
button {
  font-weight: 700;
  width: 200px;
  height: 100px;
  display:flex;
  justify-items: center;
}
</style>
