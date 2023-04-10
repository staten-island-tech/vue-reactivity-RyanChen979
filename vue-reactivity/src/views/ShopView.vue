<script setup>
import Card from "../components/ShopList.vue";
import { computers } from "../ItemsList";
</script>

<template>
  <main class="card">
    <Card
      v-for="computer in computers"
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
