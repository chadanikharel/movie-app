<template>
    <div class="grid sm:grid-cols-3 gap-7 m-10">
        <div class="bg-white rounded-lg shadow-md overflow-hidden">
            <img class=" w-full object-cover" :src="`https://image.tmdb.org/t/p/w300`+ movie.poster_path" alt="Placeholder Image"/>
       </div>
       <div class="sm:col-span-2 mx-6">
        <h1 class="font-bold text-2xl mb-5">{{ movie.title }}</h1>
        <h3 class="font-semibold text-lg mb-5">Release Date: {{ movie.release_date }}</h3>
        <p class="text-gray-500 text-md mb-8"> {{ movie.overview }} </p>
        <p class="text-gray-500 text-md">Revenue: $ {{ movie.revenue }}</p>
        <div class="mt-6">
            <NuxtLink to="https://www.youtube.com/" target="_blank" class="bg-cyan-900 hover:bg-cyan-950 text-white font-medium py-2 px-4 rounded"> Watch Trailer </NuxtLink>
            <button class="bg-rose-500 hover:bg-rose-600 text-white font-medium py-2 px-4 rounded m-5"> Buy Now </button>
        </div>
        </div>
    </div>
</template>

<script lang="ts" setup>
import {Movie} from '@/types/types'
    defineProps<{movie:Movie}>();
    
</script>

<style scoped>
   
</style>