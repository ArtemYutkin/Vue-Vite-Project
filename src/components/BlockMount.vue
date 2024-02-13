<script setup>
import { reactive, ref } from 'vue';
// const count = ref(0);
const counter = reactive({
    count: 100
});
const Plus = () => {
    counter.count+=5
}
</script>

<template>
    <button @click="Plus()">
        Count:
        <span>{{ counter.count }}</span>
    </button>
    <button @click="counter.count = 100">
        reset
    </button>
</template>