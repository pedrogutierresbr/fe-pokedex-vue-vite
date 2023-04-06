<script setup>

const pokemon = defineProps(['name'])

</script>

<template>
    <div>
        <div class="card">
            {{ pokemon.name }}
        </div>
    </div>
</template>