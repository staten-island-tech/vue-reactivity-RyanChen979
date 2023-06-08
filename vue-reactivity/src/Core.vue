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

        <h3>Total Price: ${{ Price.totalPrice }}</h3>
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
  padding-top: 5rem;
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
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}
</style>
