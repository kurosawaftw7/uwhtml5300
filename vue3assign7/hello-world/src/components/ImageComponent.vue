<template>
    <div>
        <h1>{{msg}}</h1>
        <img :alt="alt" :src="image">
    </div>
  </template>
  
  <script>
  export default {
    name: 'ImageComponent',
    props: {
      msg: String, 
      image: String,
      alt: String,

    }
  }
  </script>
  
  <!-- Add "scoped" attribute to limit CSS to this component only -->
  <style scoped>
  
  </style>
  