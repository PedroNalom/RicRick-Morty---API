<script setup>
import { onMounted, reactive, ref } from 'vue';
import ListCharacters from '../components/ListCharacters.vue';

let characters = reactive(ref());

onMounted(() => {
  fetch("https://rickandmortyapi.com/api/character")
  .then(response => response.json())
  .then(response => {
    characters.value = response.results
    console.log(characters)
  })
})
</script>

<template>
  <main>
    <div class="container">
        <div class="col-sm-12">
          <div class="card">
            <div class="card-body row">
              <ListCharacters  v-for="character in characters" 
            :key="character.name" 
            :name="character.name"
            :status="character.status"
            :species="character.species"
            :gender="character.gender"
            :location="character.location"
            :episode="character.episode"
            :url="character.url"
            />
            </div>
          </div>
        </div>
      </div>
  </main>
</template>
