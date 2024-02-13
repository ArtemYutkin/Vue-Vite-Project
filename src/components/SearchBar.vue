<script setup>
import { ref, computed } from 'vue'

const utilitys = ref([
    'Hammer',
    'Scissors',
    'CrowBar',
    'Nails',
    'Pins',
    'MultyTool',
])

const query = ref('')

const queryUtilitys = computed(() => {
    return utilitys.value.filter((utility) => utility.indexOf(query.value) !== -1);

})
</script>

<template>
    <div>
        <input type="search"
        placeholder="Type util name"
        v-model="query"
        >
        <ul>
            <li v-for="utility in queryUtilitys" 
            :key="utility"
            >
                {{ utility }}
            </li>
        </ul>
    </div>
</template>