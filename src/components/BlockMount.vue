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
    <div class="BlockMount">
        <button @click="Plus()">
            Count:
            <span>{{ counter.count }}</span>
        </button>
        <button @click="counter.count = 100">
            reset
        </button>
    </div>
</template>

<style scoped>
.BlockMount {
    height: 100px;
    width: 300px;
}
</style>