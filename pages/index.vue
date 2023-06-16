<template>
    <div>
        <Banner />
        <Search />
        <div class="grid md:grid-cols-2 lg:grid-cols-4 sm:grid-cols-1 justify-items-center">
           <div v-for="movie in 8">
            <MoviePoster :movieid="movieid" :title="title" :date="date" :poster="poster" />
            </div> 
        </div>
    </div>
</template>

<script setup>
    const movieid = ref(1);
    const title = ref("X FAST");
    const date = ref("3 june, 2023");
    const poster = ref("https://image.tmdb.org/t/p/w500/1E5baAaEse26fej7uHcjOgEE2t2.jpg");
</script>

<style scoped>

</style>