<template>
    <div>
        <header class="shadow-sm py-5 px-5">
            <h3>
                <NuxtLink class="font-bold text-xl">Nuxt Products</NuxtLink>
            </h3>
        </header>
    </div>

    <div>
        <slot />
    </div>

    <footer>
        <nav>
            <ul class="container p-4 flex gap-5">
                <li>
                    <NuxtLink to="/">Home</NuxtLink>
                </li>
                <li>
                    <NuxtLink to="/about">About</NuxtLink>
                </li>
                <li>
                    <NuxtLink to="/products">products</NuxtLink>
                </li>
            </ul>
        </nav>
    </footer>
</template>