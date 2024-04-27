<script setup>
const character = defineProps(["name", "url", "status", "species", "gender", "location", "episode"])
const characterId = character.url.split('/')[5]
const imageUrl= "https://rickandmortyapi.com/api/character/avatar/" + characterId + ".jpeg"
console.log(imageUrl)

</script>

<template>  
    <div class="col-md-4">
        <div class="card p-2 mb-3">
            <img :src="imageUrl" height="250" alt="">
            <p class="text-center">Nome: {{character.name}}</p>
            <p class="text-center">Status: {{character.status}}</p>
            <p class="text-center">Espécie: {{character.species}}</p>
            <p class="text-center">Gênero: {{character.gender}}</p>
            <p class="text-center">Localização: {{character.location.name}}</p>
            <p class="text-center">Número de episódios presente: {{character.episode.length}}</p>
        </div>
    </div>
</template>

<style>

</style>