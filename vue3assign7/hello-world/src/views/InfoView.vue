<template>
<h1>This is the info page</h1>
<div class="accordion" id="accordionExample">
  <div class="accordion-item" v-for="(movie, key) in movies" :key="key">
    <h2 class="accordion-header">
      <!-- accordion and movie title code -->
      <button class="accordion-button" type="button" data-bs-toggle="collapse" :data-bs-target="'#collapse' + key" aria-expanded="true" aria-controls="collapseOne">
        {{ movie.Title }}
      </button>
    </h2>
    <!-- insert of array info -->
    <div :id="'collapse' + key" class="accordion-collapse collapse" data-bs-parent="#accordionExample">
      <div class="accordion-body">
        {{ movie.Genre }}
        {{ movie.Year }}
        {{ movie.Runtime }}
      </div>
    </div>
  </div>


</div>

</template>

<script>
// array for movie info
export default {
  data() {
    return {
      movies: [
        {Title: 'The Seven Samurai', Genre: 'Genre: Epic Adventure', Year: 'Year of Release: 1954', Runtime: 'Runtime: 3 hours and 27 minutes'},
        {Title: 'Ikiru', Genre: 'Genre: Humanist Drama', Year: 'Year of Release: 1952', Runtime: 'Runtime: 2 hours and 23 minutes'},
        {Title: 'Ran', Genre: 'Genre: Epic Action', Year: 'Year of Release: 1985', Runtime: 'Runtime: 2 hours and 40 minutes'},
    ] 
    };
  },
};
</script>
