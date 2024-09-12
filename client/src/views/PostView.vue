<template>
    <article>
        {{ post.body }}
    </article>
</template>


<script setup>
    import { useRoute } from 'vue-router'
    import { ref } from "vue"
    fetch('https://dummyjson.com/posts')
    .then(res => res.json())
    // .then(res => posts.value = res.post )
    .then(console.log)

    const route = useRoute()
    const id = parseInt(route.params.id)
    console.log(id)

    const post = ref()
    

</script>