<script setup lang="ts">
    import { PriceItem } from '../types/interfaces'

    interface Props {
        items: PriceItem[]
    }
const props = defineProps<Props>()
</script>

<template>
    <div v-for="item in items">
        {{ item.kitchen }}
    </div>
  </template>

<style>
</style>