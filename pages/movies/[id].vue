<template>
    <div>
        <MovieDetail :movie="movie"/>
    </div>
</template>

<script setup>
    const route = useRoute()
    const {data:movie} = useFetch(`https://api.themoviedb.org/3/movie/${route.params.id}?api_key=135e910b71d49a040b1b680c82e244e6`)
</script>

<style scoped>

</style>