<template>
   <li class="post" v-for="(post,index) in posts" :key="post.id">
    <h3>{{ posts.title }}</h3>
    <img src="" alt="">
    <ul class="tags">
        <li class="tag" v-for="tag in post.tags" :key="tag.id">
            {{ tag }}
        </li>
    </ul>
    <RouterLink :to="'/product/' +(index +1)">читать подробнее</RouterLink>
   </li>
  </template>
<style scoped>

.post{
    background-color: bisque;
    color: brown;
    padding: 10px;
    display: flex;
    height: ;
    flex-direction: column;
    gap: 10px;
}
.tags{
    display: flex;
    gap: 10px;

}
a{
    padding: 10px;
    background-color: brown;
    text-decoration: none;

}
</style>

<script setup>
    import { ref } from "vue"
    fetch('https://dummyjson.com/posts')
    .then(res => res.json())
    .then(res => posts.value = res.posts)

</script>