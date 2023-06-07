<script setup>
import TheHeader from './components/TheHeader.vue'
import TheMenu from './components/TheMenu.vue'
import TheFooter from './components/TheFooter.vue'
</script>

<template>
  <div
    class="min-h-screen border-b-[1.6rem] border-b-[#edc84b] bg-[#f7f2e9] p-[3.2rem] pb-24 text-[#252525]"
  >
    <div class="mx-auto flex max-w-7xl flex-col items-center gap-[4.8rem]">
      <TheHeader />
      <TheMenu />
      <TheFooter />
    </div>
  </div>
</template>
