<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import { ref } from 'vue'

const count = ref(0)

const increment = () => {
  console.log("clicked")
  count.value++
}

const songs = [
  {
    "title": "Bohemian Rhapsody",
    "artist": "Queen",
    "album": "A Night at the Opera",
    "year": 1975,
    "genre": "Rock",
    "duration_seconds": 355
  },
  {
    "title": "Billie Jean",
    "artist": "Michael Jackson",
    "album": "Thriller",
    "year": 1982,
    "genre": "Pop",
    "duration_seconds": 294
  },
  {
    "title": "Like a Rolling Stone",
    "artist": "Bob Dylan",
    "album": "Highway 61 Revisited",
    "year": 1965,
    "genre": "Rock",
    "duration_seconds": 369
  },
  {
    "title": "Shape of You",
    "artist": "Ed Sheeran",
    "album": "÷ (Divide)",
    "year": 2017,
    "genre": "Pop",
    "duration_seconds": 233
  },
  {
    "title": "Smells Like Teen Spirit",
    "artist": "Nirvana",
    "album": "Nevermind",
    "year": 1991,
    "genre": "Grunge",
    "duration_seconds": 301
  }
]

</script>

<template>
<div>
  <p class="">test</p>
</div>
</template>

<style scoped>

</style>
