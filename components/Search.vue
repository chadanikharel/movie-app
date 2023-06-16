<template>
    <div class="container mx-auto md:px-40 mt-5">
        <form>  
            <div class="relative">
                <div class="absolute inset-y-0 left-0 flex items-center pl-3 pointer-events-none">
                    <svg aria-hidden="true" class="w-5 h-5 text-gray-500 dark:text-gray-400" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z"></path></svg>
                </div>
                <input type="search"  class="w-full p-3 focus:outline-none pl-10 text-sm text-gray-900 border border-gray-400 rounded-lg bg-gray-100 focus:ring-1 focus:ring-gray-400" placeholder="Search..." required>
                <button type="submit" class="text-white absolute right-2.5 bottom-1.5 bg-cyan-900 hover:bg-cyan-950 focus:ring-4 focus:outline-none font-medium rounded-lg text-sm px-4 py-2">Search</button>
            </div>
        </form>
    </div>
</template>

<script setup>

</script>

<style lang="scss" scoped>

</style>