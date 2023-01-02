<template>
    <div>
        <header class="shadow-sm bg-white">
            <nav class="container mx-auto p-4">
                <NuxtLink to="/products" class="font-bold">Nuxt Dojo Merchant</NuxtLink>
            </nav>
        </header>

        <!-- output the page content -->
        <siv class="container mx-auto p-4 flex justify-between border-t-2">
            <slot />
        </siv>

        <footer class="container mx-auto p-4 flex justify-between border-t-2">
            <div>
                <ul class="flex gap-4">
                    <li>
                        <NuxtLink to="/">Home</NuxtLink>
                    </li>
                    <li>
                        <NuxtLink to="/about">About</NuxtLink>
                    </li>
                    <li>
                        <NuxtLink to="/products">Products</NuxtLink>
                    </li>
                </ul>
            </div>
        </footer>
    </div>
</template>

<style scoped>
.router-link-exact-active {
    color: #12b488;
}
.ul.no-bullets {
    list-style-type: square;
    padding: 0;
    margin: 0;
}
</style>
