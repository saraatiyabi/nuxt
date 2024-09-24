<script setup>
const props = defineProps({
    product: Object
})

const { product } = props;
</script>

<template>
    <div class="card text-center">
        <img class="thumb" :src="product.image" alt="product" />
        <h2>{{ product.title }}</h2>
        <button class="btn my-4">
            <NuxtLink :to="`/products/${product.id}`">View More</NuxtLink>
        </button>
    </div>
</template>


<style scoped>
.thumb {
    max-height: 220px;
    max-width: 70%;
    margin: 0 auto;
}
</style>