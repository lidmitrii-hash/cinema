<script setup>

import AppHeader from './components/AppHeader.vue'
import AppNav from './components/AppNav.vue'
import AppSchedule from './components/AppSchedule.vue'
import AppCardList from './components/AppCardList.vue'
import AppFooter from './components/AppFooter.vue'

import { ref, onMounted } from 'vue'


const movies = ref([])
const days = ref([])

onMounted(async () => {
  try {
    const [moviesRes, daysRes] = await Promise.all([
      fetch('https://9a307c907308615f.mokky.dev/movies'),
      fetch('https://9a307c907308615f.mokky.dev/days')
    ])

    movies.value = await moviesRes.json()
    days.value = await daysRes.json()
  } catch (error) {
    console.error(error)
  }
})

</script>





<template>
<div class="w-[1240px] m-auto h-[2000px] bg-white">


  <img src="/header.png" class="w-full h-[380px]" />
  <AppHeader />
  <AppNav />
  <AppSchedule :days="days" />
  <AppCardList :items="movies" />
  <AppFooter />


</div>
</template>




<style scoped>

</style>
