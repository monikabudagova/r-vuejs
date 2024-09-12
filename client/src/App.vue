<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <header>
      <nav>
        <RouterLink to="/">Главная</RouterLink>
        <RouterLink to="/about">Обо мне</RouterLink>
        <RouterLink to="/about">Блог</RouterLink>
      </nav>
  </header>

  <RouterView />
</template>

<style scoped>

</style>
