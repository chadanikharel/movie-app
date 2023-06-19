<template>
    <div>
        
        <MovieDetail
      :title="title"
      :date="date"
      :poster="poster"
      :revenue="revenue"
      :overview="overview"
    />
    </div>
</template>

<script>
    const route = useRoute();
    console.log('route :', route.params.id)
    const {data: movie} = await useFetch("http://api.themoviedb.org/3/movie/now_playing?api_key=135e910b71d49a040b1b680c82e244e6/movies/${route.params.id}")  
    console.log("movie",movie)
</script>

<style scoped>

</style>