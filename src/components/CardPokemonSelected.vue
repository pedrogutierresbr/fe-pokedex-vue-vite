<script setup>

const pokemon = defineProps(["name", "xp", "height", "image", "loading"])

</script>

<template>
    <div class="card cardSelected" :class="loading ? '' : 'animate__animated animate__flipInY'">
        <img :src="pokemon.image" class="card-img-top pt-2" :alt="pokemon.name" height="250">
        <div class="card-body">
            <h5 class="pokemonName card-title text-center">{{ pokemon.name }}</h5>
            <hr>
            <div class="row">
                <section class="col">
                    <strong>XP: </strong>
                    <span>{{ pokemon.xp }}</span>
                </section>

                <section class="col">
                    <strong>Altura: </strong>
                    <span>{{ pokemon.height }}</span>
                </section>
            </div>
        </div>
    </div>
</template>

<style scoped>
.cardSelected {
    height: 450px;
    background: rgb(72, 63, 251);
    background: radial-gradient(circle, rgba(72, 63, 251, 0.5) 0%, rgba(70, 252, 244, 0.3) 100%);
}

.pokemonName {
    text-transform: capitalize;
}
</style>