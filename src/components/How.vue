<script setup>
import { ref } from 'vue'

const users = ref([
    {id: 1, name: 'Tommy', age: 22},
    {id: 2, name: 'Viktor', age: 43},
    {id: 3, name: 'Valery', age: 21},
    {id: 4, name: 'Vivien', age: 65},
])
</script>

<template>
    <div>
        <ul>
            <li v-for="user in users" 
            :key="user.id"
            >
                {{ user.name }}, {{ user.age }} y.o.
            </li>
        </ul>
    </div>
</template>
