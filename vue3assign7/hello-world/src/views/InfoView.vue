<template>
<h1>This is the info page</h1>
<div class="accordion" id="accordionExample">
  <div class="accordion-item" v-for="(movie, key) in movies" :key="key">
    <h2 class="accordion-header">
      <button class="accordion-button" type="button" data-bs-toggle="collapse" :data-bs-target="'#collapse' + key" aria-expanded="true" aria-controls="collapseOne">
        {{ movie.Title }}
      </button>
    </h2>
    <div :id="'collapse' + key" class="accordion-collapse collapse" data-bs-parent="#accordionExample">
      <div class="accordion-body">
        {{ movie.Description }}
      </div>
    </div>
  </div>


</div>

</template>

<script>
export default {
  data() {
    return {
      movies: [
        {Title: 'The Seven Samurai', Description: 'Description of movie'},
        {Title: 'Ikiru', Description: 'Description of movie'},
        {Title: 'Ran', Description: 'Description of movie'},
    ] 
    };
  },
};
</script>
