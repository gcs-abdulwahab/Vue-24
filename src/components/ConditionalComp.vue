<template>
    <h1> Conditional Component </h1>
    <div v-if="showDiv">This div will be hidden after 2 seconds</div>
    <div v-else>This div will be shown after 2 seconds</div>




</template>

<script setup>

import { ref } from 'vue'

const showDiv = ref(true)

setInterval(() => {
    showDiv.value = !showDiv.value
}, 2000)

</script>

<style></style>