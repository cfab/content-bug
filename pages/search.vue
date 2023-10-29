<template>
  <div>
    <NuxtLink to="/">go back home</NuxtLink>
    <h1>Search</h1>

    <input class="border" v-model="search">
    {{ search }}

    <pre>{{ results }} </pre>
  </div>
</template>

<script lang="ts" setup>
import {computed} from 'vue'
const search  = ref('')
const results = await searchContent('laboris') // hardcoded but should be search.value
</script>

<style>
/* input: {
  border: 1px solid #ccc;
} */
</style>
