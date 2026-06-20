<script setup>
import AppCard from './AppCard.vue'

defineProps({
  items: Array
})
</script>


<template>
   <div class="grid grid-cols-4 bg-white pl-10 pt-6 pb-5">
    <AppCard
      v-for="movie in items"
      :key="movie.id"
      :movie="movie"
    />
  </div>
</template>


