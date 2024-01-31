<template>
  <div class="about">
    <h1>This is the movie poster page</h1>
  </div>
  <div id="app">
    <!-- <figure v-for="movie in './src/assets/Seven_Samurai_poster.jpg'" :key="key">
      <img v-bind:src="movie.Poster">
      <figcaption>{{ movie.Poster }}</figcaption> -->
      <div class="posters">
        <img v-for="(movie, key) in movies" :key=key :alt="movie.Title" :src="movie.Poster"/>
      </div>
        </div>
  
  <div>

    <script>
export default {
  data() {
    return {
    //   movies: [
    //     // {Title: 'The Seven Samurai', Poster: './src/assets/Seven_Samurai_poster.jpg'},
    //     // {Title: 'Ran', Poster: './src/assets/Ran-Vintage-Movie-Poster-Original-Japanese-1-panel-20x29.jpg'},
    //     // {Title: 'Ikiru', Poster: './src/assets/Ikiru_poster.jpg'},
    // ] 
    movies: [
        {Title: 'The Seven Samurai', Poster: require('../assets/Seven_Samurai_poster.jpg')},
        {Title: 'Ikiru', Poster: require('../assets/Ran-Vintage-Movie-Poster-Original-Japanese-1-panel-20x29.jpg')},
        {Title: 'Ran', Poster: require('../assets/Ikiru_poster.jpg')},
    ]
    };
    };
  },


app.mount('#app')

</script>
  </div>
</template>
