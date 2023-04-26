<script setup>
import ProductCard from './components/ProductCard.vue';
</script>

<template>
  <header>
    <h1 class="text font-bold text-center text-4xl py-2">Product</h1>
  </header>
  <main class="grid grid-cols-2 lg:grid-cols-4 gap-3 px-3">
    <ProductCard title="Magic Socks" materials="50% cotton" price="15"/>
    <ProductCard title="Black Jeans" materials="80% cotton" price="26"/>
    <ProductCard title="White Jumper" materials="80% cotton" price="37"/>
    <ProductCard title="Blue Jean Jacket" materials="80% cotton" price="41"/>
    <div>Total: $0</div>
  </main>
</template>
