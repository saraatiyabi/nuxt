<template>
    <div class="w-full h-screen flex justify-center items-center flex-col">
        <h1 class="my-7 text-[80px] font-bold">{{ error.statusCode }}</h1>
        <p class="text-2xl uppercase mb-5">Ooops!</p>
        <p class="text-xl text-gray-600">{{ error.message }}</p>

        <button class="btn" @click="removeErrorHandler">
            Go Back
        </button>
    </div>
</template>

<script setup>
const props = defineProps({
    error: Object
})

const { error } = props;

const removeErrorHandler = () => clearError({ redirect: "/" })
</script>

<style lang="scss" scoped></style>