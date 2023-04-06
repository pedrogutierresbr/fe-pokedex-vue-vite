<script setup>

const pokemon = defineProps(['name', 'urlBaseSVG'])

</script>

<template>
    <div class="col-4">
        <div class="card p-2 mb-3 cardListPokemons">
            <p class="text-center">{{ pokemon.name }}</p>
            <img :src="urlBaseSVG" class="card-img-top" :alt="pokemon.name" height="80" />
        </div>
    </div>
</template>

<style scoped>
.cardListPokemons {
    background: rgb(72, 63, 251);
    background: radial-gradient(circle, rgba(72, 63, 251, 0.5) 0%, rgba(70, 252, 244, 0.3) 100%);
    cursor: pointer;
}

.cardListPokemons:hover {
    background: rgb(72, 63, 251);
    background: radial-gradient(circle, rgba(72, 63, 251, 0.6) 0%, rgba(70, 252, 244, 0.4) 100%);
    cursor: pointer;
}

.cardListPokemons img:hover {
    padding: .1rem;
}
</style>