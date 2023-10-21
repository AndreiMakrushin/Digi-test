<script setup>
import { ref, onMounted, onBeforeUnmount } from "vue";
import Button from "../ui/buttons/ButtonCatalog.vue";
import ButtonMobile from "../ui/buttons/ButtonMobile.vue";
import Logo from "../ui/Logo/Logo.vue";
import Search from "../ui/Search-panel/Search.vue";
import MobileSearch from "../ui/Search-panel/MobileSearch.vue";
import Navigation from "../ui/navigation/Navigation.vue";

const input = ref("");
const mobile = ref(false);

const handleResize = () => {
  mobile.value = window.innerWidth < 768;
};

onMounted(() => {
  window.addEventListener("resize", handleResize);
});

onBeforeUnmount(() => {
  window.removeEventListener("resize", handleResize);
});
handleResize();
</script>
<template>
  <div class="header">
    <div class="logo">
      <Logo />
      <Button text="Каталог" />
    </div>
    <div class="search">
      <Search
        v-if="!mobile"
        type="text"
        placeholder="Поиск по 100 000 товаров "
        v-model="input"
      />
      <div class="mobile-search" v-else>
        <div class="search-btn">
          <MobileSearch type="text" placeholder="Запрос" v-model="input" />
          <ButtonMobile />
        </div>
        <div class="line"></div>
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
  align-items: center;
}
.search-btn{
  margin-bottom: 6px;
  display: flex;
  align-items: center;
  width: 100%;
  flex-direction: row;
}
.mobile-search {
  display: flex;
  flex-direction: column;
  align-items: end;
  width: 100%;
}

@media (max-width: 768px) {
  .line {
    right: 0;
    border: 1px solid #d5d5d5;
    width: 90%;
  }
  .logo {
    display: none;
  }
  .navigation {
    display: none;
  }

  .search {
    gap: 10px;
  }
}
</style>
