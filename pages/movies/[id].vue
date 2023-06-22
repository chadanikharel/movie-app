<template>
    <div>
        <MovieDetail :title="movie.title" :release_date="movie.release_date" :poster="movie.poster_path" :revenue="movie.revenue" :overview="movie.overview" />
    </div>
</template>

<script setup>
    const route = useRoute()
    const {data:movie} = useFetch(`https://api.themoviedb.org/3/movie/${route.params.id}?api_key=135e910b71d49a040b1b680c82e244e6`)
</script>

<style scoped>

</style>