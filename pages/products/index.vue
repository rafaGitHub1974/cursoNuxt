<template>
    <div>
        <h1>
            Estás en la página de productos SIN ID
        </h1>
        <nuxt-link :to="'/products/' + id">product 1</nuxt-link>
        <nuxt-link to="/products/2">product 2</nuxt-link>
        <button @click="$router.push('/')"></button>
    </div>    
</template>
<script>
export default {
    data() {
        return {
            id: 1,
        }
    },
}
</script>