<!-- Component Madness is all about visualizing components as objects on the web page and how they inter-relate and communicate -->
<script setup>
import AlvinComponent from '../components/madness/AlvinComponent.vue'
import { ref } from 'vue'

const myNumber = ref(null)

const handleEmit = () => {}
</script>

<template>
  <div class="container bg-purple-300 p-6 text-center">
    <h1 class="font-bold text-xl p-4">Component Madness</h1>

    <p class="mb-2">My number: {{ myNumber ? myNumber.value : "I don't know!" }}</p>
    <AlvinComponent @button-emit="handleEmit" />
  </div>
</template>

<style scoped></style>
