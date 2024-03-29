<script setup>
import { onMounted, ref } from 'vue';
import { computed } from 'vue';
const count = ref(0);
const step = ref(1);


const decrement = () => {
    count.value -= step.value;
}

const increment = () => {
    //  parseInt() function parses a string and returns an integer.
    count.value += parseInt(step.value);

    
}


//  computed property that will square the
//  value of count
const squared = computed(() => count.value * count.value);
const stepSquared = computed(() => step.value * step.value);
</script>
<template>

    <h1>Convertor :{{ count }}</h1>
    
    <input type="text" v-model="count">
    <br>
    Step: <input type="text" v-model="step" />
    <button @click="increment">Increment</button>
    <button @click="decrement">Decrement</button>
</template>

<style></style>