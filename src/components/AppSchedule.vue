<script setup>
defineProps({
  days: Object
})
</script>


<template>
<div class="bg-[#F2F2F5] flex items-center h-[55px]">
    <ul class="flex gap-2 overflow-x-auto whitespace-nowrap ml-10">
      <li v-for="day in days" :key="day.id">
        <button
          class="h-9 px-3 rounded-full flex items-center justify-center cursor-pointer"
          :class="day.active ? 'bg-[#E92B43] text-white' : 'bg-white text-black'"
          @click="setActive(day.id)"
        >
          {{ day.label }}
        </button>
      </li>
    </ul>
  </div>
</template>

<style scoped>
</style>
