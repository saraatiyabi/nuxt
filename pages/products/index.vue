<script lang="ts" setup>
definePageMeta({
    layout: "products"
})

const { data: products } = await useFetch("https://fakestoreapi.com/products");
</script>

<template>
    <h1 class="p-5 font-bold text-xl">Products</h1>
    <div class="grid grid-cols-4 px-5 py-5 gap-5">
        <div v-for="product in products">
            <ProductCard :product="product" />
        </div>
    </div>
</template>

<style lang="postcss" scoped></style>
