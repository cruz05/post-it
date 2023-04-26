<script setup>
import { ref } from 'vue';

defineProps({
    title: String,
    materials: String,
    price:Number
})

const counter = ref(0)

</script>

<template>
<div class="text-green-600 rounded-md border-2 border-gray-300 p-3 text-lg">
    <h2 class="font-semibold text-3xl">{{ title }}</h2>
    <span>${{ price }}</span>
    <p>{{ materials }}</p>
    <div v-if="counter > 0">
        <button class="border px-3 font-semibold" @click="() => counter--">-</button>
        <span class="px-2">{{counter }}</span> 
        <button class="border px-3 font-semibold" @click="() => counter++">+</button>
    </div>
    <button v-else @click="counter = 1" class="px-3 py-1 border-2 rounded-sm">Add to Cart</button>
</div>
</template>