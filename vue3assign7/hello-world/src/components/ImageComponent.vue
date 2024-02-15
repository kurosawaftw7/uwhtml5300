<template>
    <div>
      <!-- HTML and image code -->
        <h1>{{msg}}</h1>
        <img :alt="alt" :src="image" :title="title" @click="toggleBorder()">
    </div>
  </template>
  
  <script>
  import toggleBorder from "../mixins/mixin.js"
// JS creating the mixin
  export default {
    name: 'ImageComponent',
    props: {
      msg: String, 
      image: String,
      alt: String,
      title: String,
    },
    mixins: [toggleBorder]
  }
// border toggle code
  const toggleBorder = {
    data() {
      return {
        isHidden: false
      }
    },
    methods: {
      toggleBorder() {
        this.isHidden = !this.isHidden;
      }
    }
  }
  </script>
  
  <!-- Add "scoped" attribute to limit CSS to this component only -->
  <style scoped>
    .image-border { 
      border: 5px solid black;
    } 
  </style>
  