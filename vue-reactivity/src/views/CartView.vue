<script setup>
import Card from "../components/CartList.vue";
import { cartList } from "../cartList.js";
</script>

<template>
  <main class="card">
    <Card
      v-for="computer in cartList.list"
      :name="computer.name"
      :price="computer.price"
      :image="computer.image"
      :processor="computer.processor"
      :memory="computer.memory"
      :harddrive="computer.harddrive"
      :color="computer.color"
    />
  </main>
</template>

<style>
.card {
  display: flex;
  flex-wrap: wrap;
  flex-direction: row;
  justify-content: space-between;
}
</style>
