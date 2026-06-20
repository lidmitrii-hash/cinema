<script setup>
defineProps({
  movie: Object
})
</script>

<template>
  <div class="w-[267px] bg-white rounded overflow-hidden shadow">

    <img
      :src="movie.imageUrl"
      class="w-[265px] h-[384px] object-cover"
    />

    <div class="p-2">
      <h2 class="font-semibold text-lg">{{ movie.title }}</h2>
      <div class="flex flex-wrap gap-1 mb-2">
        <span
          v-for="(genre, index) in movie.genres"
          :key="index"
          class="text-xs text-gray-500 bg-[#F2F2F5] mt-2 px-2 py-0.5 rounded"
        >
          {{ genre }}
        </span>
      </div>

    </div>

    <div class="p-2 grid grid-cols-3 gap-4">
      <div
        v-for="item in movie.times"
        :key="item.time"
        class="flex flex-col items-center w-16"
      >

        <span class="bg-[#E92B43] items-center text-white font-semibold text-sm rounded-t px-4 py-0.5 w-full cursor-pointer">
          {{ item.time }}
        </span>


        <span v-if="item.price" class="bg-white border border-t-0 border-[#E92B43] text-gray-800 text-[10px] font-semibold px-2 py-0.5 w-full cursor-pointer">
          {{ item.price }}
        </span>


        <span v-if="item.hall" class="text-[10px] text-gray-400 px-2 py-0.5">
          {{ item.hall }}
        </span>

      </div>
    </div>

  </div>

</template>


