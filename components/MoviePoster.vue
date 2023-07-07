<template>
    
    <div class="bg-gray-100 rounded-lg shadow-lg overflow-hidden m-4 p-2">
        <div class="px-2 py-4">
            <p class="font-semibold text-md mb-2 text-center">{{ movie.title }}</p>
            <div class="bg-red-400 mb-4">
                <img :src="`https://image.tmdb.org/t/p/w300`+movie.poster_path" class="h-400 w-300 object-cover"/>
            </div>
        <p class="text-gray-500 text-sm m-2 ">Release date: {{ movie.release_date }}</p>
        
        <div class="mt-4 p-2 text-right">
        <NuxtLink :to="`movies/${movie.id}`" class="bg-rose-500 hover:bg-rose-600 text-white font-medium py-2 px-4 rounded">Get Details</NuxtLink>
        </div>
    </div>
    </div>

</template>
    
<script lang="ts" setup>
    import {Movie} from '@/types/types'
    defineProps<{movie:Movie}>();


</script>

<style scoped>
    .h-400{
        height: 350px;
    }
    .w-300{
        width: 300px;
    }
</style>