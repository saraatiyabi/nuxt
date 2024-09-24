<script setup>
const props = defineProps({
    product: Object
})

const { product } = props;
</script>

<template>
    <div class="card">
        <section class="container w-full h-screen grid grid-cols-2 gap-10">
            <div class="p-7">
                <img :src="product.image" class="w-[400px] mx-auto my-7" />
            </div>
            <div class="pt-10 p-7 mt-10">
                <h1 class="text-4xl my-7">{{ product.title }}</h1>
                <p class="text-xl my-7">Price - ${{ product.price }}</p>
                <h3 class="font-bold border-b-2 mb-4 pb-2">Product Description</h3>
                <p class="text-gray-500 mb-7">{{ product.description }}</p>
            </div>
        </section>
    </div>

</template>


<style lang="scss" scoped>
</style>