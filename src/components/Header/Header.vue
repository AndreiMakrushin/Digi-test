<script setup>
import { ref } from "vue";
import Button from "../buttons/Button.vue";
import Logo from "../Header/Header-components/Logo/Logo.vue";
import Search from "../Header/Header-components/Search-panel/Search.vue";
import Navigation from "./Header-components/navigation/Navigation.vue";

const input = ref("");
</script>
<template>
  <div class="header">
    <div class="logo">
      <Logo />
      <Button text="Каталог" />
    </div>
    <div class="search">
      <Search
        type="text"
        placeholder="Поиск по 100 000 товаров "
        v-model="input"
      />
      <div class="mobile-button">
        <Button text="Поиск" />
      </div>
    </div>
    <div class="navigation">
      <Navigation />
    </div>
  </div>
</template>
<style scoped>
.header {
  width: 100%;
  padding: 12px 0px;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
}
.logo {
  display: flex;
  flex-direction: row;
}
.search {
  margin: 0px 20px;
  flex-grow: 1;
  display: flex;
  flex-direction: row;
}
.search .mobile-button{
  display: none;
}
@media (max-width: 768px) {
  .logo {
    display: none;
  }
  .navigation {
    display: none;
  }
  .search .mobile-button{
    display: block;
  }
  .search {
    gap: 10px;
  }
}
</style>
