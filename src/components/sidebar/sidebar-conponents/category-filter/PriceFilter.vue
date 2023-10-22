<script setup>
  import ContainerInput from '../../../ui/filter-input/ContainerInput.vue';
</script>
<template>
  <div class="price-container">
    <div class="header">
      <h1>Цена</h1>
    </div>
    <div class="input-price">
      <ContainerInput span="от" value="5 500" />
      <div class="line"></div>
      <ContainerInput  span="до" value="10 000"/>
    </div>
  </div>
</template>
<style scoped>
.price-container {
  margin-top: 28px;
  width: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
.price-container h1 {
  font-size: 16px;
  line-height: 20px;
  font-weight: 700;
}
.input-price {
  height: 36px;
  margin-top: 16px;
  display: flex;
  flex-direction: row;
  align-items: center;
}
.line {
  margin: 0 16px;
  width: 10px;
  height: 1px;
  background-color: #d5d5d5;
}
</style>
