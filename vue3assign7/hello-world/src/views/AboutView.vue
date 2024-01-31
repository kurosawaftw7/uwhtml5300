<template>
  <div class="about">
    <h1>This is the movie poster page</h1>
  </div>
  <div>
    <!-- loop for  -->
      <div class="posters">
        <img v-for="(movie, key) in movies" :key=key :alt="movie.Title" :src="movie.Poster"/>
      </div>
        </div>
  
  </template>
  <script>
  export default {
    data() {
      return {
      // array for images and titles
      movies: [
          {Title: 'The Seven Samurai', Poster: require('../assets/Seven_Samurai_poster.jpg')},
          {Title: 'Ikiru', Poster: require('../assets/Ran-Vintage-Movie-Poster-Original-Japanese-1-panel-20x29.jpg')},
          {Title: 'Ran', Poster: require('../assets/Ikiru_poster.jpg')},
      ]
      };
    }
  }


</script>