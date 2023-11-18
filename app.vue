<script setup lang="ts">
import type { PriceItem } from './types/interfaces'

  const prices = ref<PriceItem[]>([
    { _id: 1, price: 100, priceWoDiscount: 90, kitchen: 'standart', color: 'beige' },
    { _id: 2, price: 150, priceWoDiscount: 135, kitchen: 'standart', color: 'brown' },
    { _id: 3, price: 200, priceWoDiscount: 180, kitchen: 'plus', color: 'grey' },
    { _id: 4, price: 250, priceWoDiscount: 225, kitchen: 'plus', color: 'white' }])  
</script>

<template>
  <div>
    <switch-comp :items="prices"/>
  </div>
</template>
