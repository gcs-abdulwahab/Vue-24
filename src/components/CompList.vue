<template>

    <h1> This is the Comp List</h1>

    <form @submit.prevent="addTodo">
        <input v-model="newTodo" required placeholder="new todo">
        <button>Add Todo</button>
    </form>

    <ul>
        <li v-for="todo in todos" :key="todo.id">
            {{ todo.text }}
            <button @click="removeTodo(todo)">X</button>
        </li>
    </ul>

</template>

<script setup>
import { ref } from 'vue'

let id = 0
const newTodo = ref('')

const todos = ref([
    { id: id++, text: 'Learn HTML' },
    { id: id++, text: 'Learn JavaScript' },
    { id: id++, text: 'Learn Vue' }
])

const addTodo = () => {
    todos.value.push({ id: id++, text: newTodo.value })
    newTodo.value = ''
}

const removeTodo = todo => {
    console.log(todo.text)
    todos.value = todos.value.filter(t => t.id !== todo.id)
}

</script>

<style></style>