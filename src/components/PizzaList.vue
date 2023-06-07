<script setup>
import PizzaItem from './PizzaItem.vue'

defineProps(['pizzas'])
</script>

<template>
  <ul class="grid grid-cols-2 gap-[4.8rem]">
    <PizzaItem v-for="pizza in pizzas" :key="Math.random()" v-bind="pizza" />
  </ul>
</template>
