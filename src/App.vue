<script setup>
import Header from "./components/Header/Header.vue";
import Sidebar from "./components/sidebar/Sidebar.vue";
import ProductsMainContainer from "./components/product/ProductsMainContainer.vue";
</script>
<template>
  <div class="main-container">
    <div class="container">
      <div class="header">
        <Header />
      </div>
      <div class="content-container">
        <div class="sidebar">
          <Sidebar />
        </div>
        <div class="ProductsMainContainer">
          <ProductsMainContainer />
        </div>
      </div>
    </div>
  </div>
</template>
<style scoped>
.main-container {
  display: flex;
  justify-content: center;
  width: 100vw;
}
.container {
  gap: 24px;
  padding: 0px 100px 36px 100px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  width: 1920px;
}
.content-container{
  display: flex;
  gap: 24px;
  flex-direction: row;
}
.sidebar{
  width: 280px;
}
</style>
