<template>
    <div v-if="renderCard">
        <h1>Título</h1>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Tempore, sunt! Tempore unde harum repellendus nisi
            provident fuga id quia veniam natus at nulla, dolore sunt nam odio, earum ullam ut!</p>
        <button type="button" @click="closeCard">Close card</button>
    </div>
</template>

<script setup>

const props = defineProps(['renderCard']);
const eventEmitter = defineEmits(['closeCard'])

function closeCard() {
    eventEmitter('closeCard')
}
</script>

<style>

</style>