<template>
  <div class="about">
    <h1>This is the movie poster page</h1>
  </div>
  <div>
    <img v-for="'./src/assets/Seven_Samurai_poster.jpg' in movies" v-bind:src="'./src/assets/Seven_Samurai_poster.jpg'">
    <img v-for="'./src/assets/Ran-Vintage-Movie-Poster-Original-Japanese-1-panel-20x29.jpg' in movies" v-bind:src="'./src/assets/Ran-Vintage-Movie-Poster-Original-Japanese-1-panel-20x29.jpg'">
    <img v-for="'./src/assets/Ikiru_poster.jpg' in movies" v-bind:src="'./src/assets/Ikiru_poster.jpg'">
  </div>
  
  <div>
    <script>
export default {
  data() {
    return {
      movie: [
        {Title: 'The Seven Samurai', Poster: './src/assets/Seven_Samurai_poster.jpg'},
        {Title: 'Ikiru', Poster: './src/assets/Ran-Vintage-Movie-Poster-Original-Japanese-1-panel-20x29.jpg'},
        {Title: 'Ran', Poster: './src/assets/Ikiru_poster.jpg'},
    ] 
    };
  },
};
</script>
  </div>
</template>
