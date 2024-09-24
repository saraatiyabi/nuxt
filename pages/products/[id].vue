<script lang="ts" setup>
const { id } = useRoute().params;

const { data: product } = await useFetch(`https://fakestoreapi.com/products/${id}`, { key: id })

if (!product.value) {
    throw createError({ statusCode: 404, statusMessage: "Product Not Found!" })
}
</script>

<template>
    <ProductDetails :product="product" />
</template>

<style lang="postcss" scoped></style>
