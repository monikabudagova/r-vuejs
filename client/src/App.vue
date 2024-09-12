<script setup>
// import { RouterLink, RouterView } from 'vue-router'
// import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <header>
    <div class="wrapper">
      

      <nav>
        <RouterLink to="/">Главная</RouterLink>
        <RouterLink to="/about">Обо мне</RouterLink>
        <RouterLink to="/about">Блог</RouterLink>
      </nav>
    </div>
  </header>

  <RouterView />
</template>

<style scoped>

</style>
