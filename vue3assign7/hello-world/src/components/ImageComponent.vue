<template>
    <div>
        <h1>{{msg}}</h1>
        <img :alt="alt" :src="image" :title="title">
    </div>
  </template>
  
  <script>
  import mixin from "../mixins/mixin.js"

  export default {
    name: 'ImageComponent',
    props: {
      msg: String, 
      image: String,
      alt: String,
      title: String,
    },
    mixins: [mixin]
  }
  </script>
  
  <!-- Add "scoped" attribute to limit CSS to this component only -->
  <style scoped>
  
  </style>
  