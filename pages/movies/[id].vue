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
    // const movieid = ref('1');
    // const titlle = ref("X MAN");
    // const date = ref('5 june 2023');
    // const poster = ref('https://image.tmdb.org/t/p/w500/1E5baAaEse26fej7uHcjOgEE2t2.jpg');
    // const revenue = ref(5865495);
    // const overview = ref('lorem ipsum Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsam, commodi. Lorem ipsum dolor sit amet consectetur adipisicing elit. Inventore, esse.');
    const title = ref("Batman Brown City");
const date = ref("20-01-2023");
const poster = ref(
  "https://www.themoviedb.org/t/p/w600_and_h900_bestv2/74xTEgt7R36Fpooo50r9T25onhq.jpg"
);
const revenue = ref(45467545);
const overview = ref(
  "Inspired by a true story, an oddball group of cops, criminals, tourists and teens converge in a Georgia forest where a 500-pound black bear goes on a murderous rampage after unintentionally ingesting cocaine."
);

</script>

<style scoped>

</style>