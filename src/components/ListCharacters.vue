<script setup>
const character = defineProps(["name", "url", "status", "species", "gender", "location", "episode"])
const characterId = character.url.split('/')[5]
const imageUrl= "https://rickandmortyapi.com/api/character/avatar/" + characterId + ".jpeg"
console.log(imageUrl)

let coloar = 'gree'

switch(character.status){
    case "Alive":
        coloar = "green";
        break;
    case "Dead":
        coloar = "red";
        break;
    case "unknown":
        coloar = "blue";
        break;
    default:
        coloar = "black";
}

</script>

<template>  
    <div class="col-md-3">  
        <div class="card p-2 mb-3" style="height: 35rem">
            <img :src="imageUrl" height="250rem" alt="" style="margin: auto;">
            <p class="text-center">Nome: {{character.name}}</p>
            <p class="text-center" :style="{color: coloar}">Status: {{character.status}}</p>
            <p class="text-center">Espécie: {{character.species}}</p>
            <p class="text-center">Gênero: {{character.gender}}</p>
            <p class="text-center">Localização: {{character.location.name}}</p>
            <p class="text-center">Número de episódios presente: {{character.episode.length}}</p>
        </div>
    </div>
</template>

<style>

</style>
