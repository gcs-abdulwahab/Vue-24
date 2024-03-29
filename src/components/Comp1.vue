<template>
    <h1>Comp 1 : {{ username }}</h1>
    <input class="border border-slate-500 "  type="text" v-model="username"  placeholder="Type here" />


</template>

<script setup>

import { ref } from 'vue';

const username = ref("");

const textchanged = (e) => {
    username.value = e.target.value;
}


</script>

<style></style>