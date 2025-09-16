<script setup>
import { ref } from 'vue';
import MultiSelect from 'primevue/multiselect';

const cities = [
  { name: 'aaaa' },
  { name: 'aaab' },
  { name: 'aaac' },
  { name: 'aaad' },
  { name: 'aaae' },
];

let selectedCities = ref([]);
</script>

<template>
  <!-- lorem -->
  <!-- {{ cities }} -->

  {{ selectedCities }}

  <MultiSelect v-model="selectedCities" :options="cities" optionLabel="name" filter placeholder="Select Cities"
    :selectionLimit="1" class="w-full md:w-80" />
</template>

<style scoped>
</style>
