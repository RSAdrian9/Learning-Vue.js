<template>
    <div class="post-card">
        <h3>Título</h3>
        <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Reiciendis impedit iure quam hic dignissimos
            voluptatum maiores rem, libero, exercitationem error, ad vitae facilis laudantium assumenda fugit
            accusantium culpa modi non.</p>
        <PostButton />
    </div>
</template>

<script lang="ts" setup>
import PostButton from './PostButton.vue'
</script>

<style scoped>
.post-card {
    border-radius: 15px;
    padding: 10px;
    margin: 5px;
    border: 1px solid #ccc;
}
</style>