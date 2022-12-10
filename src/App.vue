<script setup>
import { ref } from 'vue'
import Card from './components/Card.vue'
let showCard = ref(false);
</script>

<template>
  <div>
    <Card :renderCard="showCard" @closeCard="showCard = false" />
    <button type="button" @click="showCard = true">Open card</button>
  </div>
</template>

<style scoped>

</style>
