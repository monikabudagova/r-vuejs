<script setup>
import { RouterLink, RouterView } from 'vue-router'
// import ShareView
</script>

<template>
  <header class="">
      <nav>
        <a href="">главная</a>
        <RouterLink to="/">Главная</RouterLink>
        <RouterLink to="/about">Обо мне</RouterLink>
        <RouterLink to="/blog">Блог</RouterLink>
      </nav>
  </header>

  <main>
    <RouterView />
  </main>

  <footer>
  все права защищены &copy; 2024
</footer>
</template>



<style scoped>
  nav{

    background-color: wheat;
    display: flex;
  }

  nav a {
    padding: 10px;
  }
  nav a:hover{
    background-color: brown;
  }
</style>
