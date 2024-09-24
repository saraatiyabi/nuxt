<template>
    <div>
        <header class="shadow-sm bg-white">
            <nav class="container mx-auto p-4 flex justify-between">
                <NuxtLink class="font-bold text-xl">Nuxt Dojo</NuxtLink>
                <ul class="flex flex-row gap-4">
                    <li>
                        <NuxtLink to="/">Home</NuxtLink>
                    </li>
                    <li>
                        <NuxtLink to="/about">About</NuxtLink>
                    </li>
                    <li>
                        <NuxtLink to="/products" class="btn">Products</NuxtLink>
                    </li>
                </ul>
            </nav>
        </header>
    </div>

    <div>
        <slot />
    </div>
</template>

<style>
.router-link-active{
    color: green;
}
</style>