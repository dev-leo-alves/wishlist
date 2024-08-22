<script setup>
import {Link, Head} from "@inertiajs/vue3";

</script>

<template>
    <div>
        <header class="bg-indigo-500 text-white">
            <nav class="flex items-center justify-between p-4 max-w-screen-lg mx-auto">
                <div class="space-x-6">
                    <Link :href="route('home')">Home</Link>
                </div>
            </nav>
        </header>
    </div>

    <main class="p-4">
        <slot />
    </main>
</template>
