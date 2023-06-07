<script setup>
defineProps(['name', 'photoName', 'ingredients', 'price', 'soldOut'])
</script>

<template>
  <li class="flex gap-14" :class="{ 'text-[#888]': soldOut }">
    <img
      :src="photoName"
      :alt="name"
      class="aspect-square w-48 self-start"
      :class="{ 'opacity-80 grayscale': soldOut }"
    />
    <div class="flex flex-col gap-3 py-2">
      <h3 class="text-[2rem]">{{ name }}</h3>
      <p class="text-[1.4rem] font-light italic">{{ ingredients }}</p>
      <span class="block text-[1.6rem]">
        {{ soldOut ? 'SOLD OUT' : price }}
      </span>
    </div>
  </li>
</template>
