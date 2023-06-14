<template>
    <div>
       <nav class="bg-cyan-900  w-full top-0 left-0">
            <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
                <div class="flex justify-between h-14">
                    <div class="sm:ml-6 sm:flex sm:items-center">
                        <NuxtLink to="/" class="text-white px-3 my-2 py-2 hover:bg-cyan-700 focus:bg-cyan-700 rounded-md ">Home</NuxtLink>
                        <NuxtLink to="/signup" class="text-white my-2 px-3 py-2 hover:bg-cyan-700 focus:bg-cyan-700 rounded-md ">Sign Up</NuxtLink>
                        <NuxtLink to="/login" class="text-white my-2 px-3 py-2 hover:bg-cyan-700 focus:bg-cyan-700 rounded-md ">Login</NuxtLink>
                        <NuxtLink to="/contact" class="text-white px-3 py-2 hover:bg-cyan-700 focus:bg-cyan-700 rounded-md ">Contact</NuxtLink>
                    </div>
                </div>
            </div>
        </nav>
    </div>
</template>

<script setup>

</script>

<style scoped>

</style>