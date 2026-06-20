<script setup>

</script>

<template>
  <div>
  <div class="bg-[#123D4B] h-[109px] flex items-center text-white mt-20">
    <img src="/Logo1.png" class="pl-10 ml-5 w-50 cursor-pointer" />
    <div class="ml-35">
      <h1 class="">admin@example.com</h1>
      <h2 class="">ticket@example.com</h2>
      <p class="font-thin text-s text-zinc-300">улица Тестовая 1</p>
    </div>

    <div  class="ml-35 mb-6">
      <div class="flex">
      <h1 class="">+7 (775) 000 00 01</h1>
      <img src="/arrow.png" class="w-2 h-2 ml-2 mt-2" />
      </div>
      <p class="font-thin text-s text-zinc-300">Касса</p>
    </div>

    <div class="ml-55 mb-6">
      <h1>08:00 - 22:00 с пн.-пт.</h1>
      <p class="font-thin text-s text-zinc-300">График работы</p>
    </div>
  </div>

  <div class="bg-[#0C3542] h-[295px] flex border-b border-[#A0AEB7]">

    <div>
    <ul class="text-white gap-10 items-center justify-center pt-8 pl-15">
      <p class="text-white text-lg font-medium">Меню</p>
      <li class="mt-5 text-lg font-thin text-zinc-300"><a href="#">Афиша</a></li>
      <li class="mt-1 text-lg font-thin text-zinc-300"><a href="#">Сеансы</a></li>
      <li class="mt-1 text-lg font-thin text-zinc-300"><a href="#">Пушкинская карта</a></li>
      <li class="mt-1 text-lg font-thin text-zinc-300"><a href="#">Кинотеатр</a></li>
      <li class="mt-1 text-lg font-thin text-zinc-300"><a href="#">Контакты</a></li>
    </ul>
    </div>

    <div class="flex flex-col ml-100 mt-8 ">
      <p class="text-white">Способы оплаты:</p>
      <div class="flex gap-5">
      <img src="/payment1.png" class="w-[60px] h-[60px] mt-3" />
      <img src="/payment2.png" class="w-[60px] h-[60px] mt-3 " />
      </div>
      <p class="text-base font-thin text-zinc-300 mt-25">Все сеансы начинаются с рекламно-информационного блока.</p>
      <p class="text-base font-thin text-zinc-300">Точную продолжительность сеансов можно уточнить в кинотеатре.</p>
    </div>

  </div>

  <div class="flex bg-[#0C3542] h-17 items-center">
    <img src="/Facebook.png" class="w-6 h-6 w-8 h-8 ml-13 cursor-pointer" />
    <img src="/Instagram.png" class="w-6 h-6 ml-3 w-8 h-8 cursor-pointer" />
    <img src="/YouTube.png" class="w-6 h-6 ml-3 w-8 h-8 cursor-pointer" />
    <img src="/VK.png" class="w-6 h-6 ml-3 w-8 h-8 cursor-pointer" />
    <p class="text-zinc-300 ml-190">© 2025 Все права защищены</p>
  </div>
  </div>
</template>
