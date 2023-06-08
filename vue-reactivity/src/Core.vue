<script setup>
import { RouterLink, RouterView } from "vue-router";
import TitleName from "./components/TitleName.vue";
import { Price } from "./totalPrice";
import { cartList } from "./cartList";
</script>

<template>
  <header>
    <div class="wrapper">
      <TitleName />

      <div class="row">
        <nav>
          <RouterLink to="/">Shop</RouterLink>
          <RouterLink to="/cart">🛒({{ cartList.length }})</RouterLink>
        </nav>

        <div class="price-display">
          <h3>Total Price: ${{ Price.totalPrice }}</h3>
        </div>
      </div>
    </div>
  </header>

  <RouterView />
</template>

<style scoped>
header {
  position: sticky;
  z-index: 1;
  top: 0;
  background-color: #221e32;
  padding-top: 3rem;
  width: 100%;
}

.row {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  padding: 1rem 0;
  margin-top: 2rem;
  font-size: 24px;
}

nav {
  text-align: center;
  text-align: left;
  margin-left: 2rem;
}
nav a {
  display: inline-block;
  padding-right: 2rem;
  border-left: 1px solid var(--color-border);
}

.price-display {
  margin-right: 2rem;
}
</style>
