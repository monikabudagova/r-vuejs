<template>
    <article>
        {{ post.body }}
    </article>
</template>


<script setup>
    // import { ref } from "vue"
    fetch('https://dummyjson.com/posts')
    .then(res => res.json())
    .then(res => 
        posts.value = res.posts
        
    )

</script>
