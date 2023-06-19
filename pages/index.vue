<template>
    <div>
        <Banner />
        <Search />
        <div class="grid md:grid-cols-2 lg:grid-cols-4 sm:grid-cols-1 justify-items-center">
           <div v-for="movie in movies.results">
            <MoviePoster :movieid="movie.id" :title="movie.title" :date="movie.release_date" :poster="movie.poster_path" />
            </div> 
        </div>
    </div>
</template>

<script setup>
    const {data:movies, error} = await useFetch("http://api.themoviedb.org/3/movie/now_playing?api_key=135e910b71d49a040b1b680c82e244e6") 
    console.log("movies:", movies)
</script>

<style scoped>

</style>