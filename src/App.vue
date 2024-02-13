<script setup>
import BlockMount from './components/BlockMount.vue';
import How from './components/How.vue';
import SearchBar from './components/SearchBar.vue';
</script>

<template>
  <div class="content-layout">
    <BlockMount></BlockMount>
    <How></How>
    <SearchBar></SearchBar>
  </div>
</template>

<style scoped>
.content-layout {
  height: 100%;
  width: 100%;
}
</style>
