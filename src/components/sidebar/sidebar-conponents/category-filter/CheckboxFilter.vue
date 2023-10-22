<script setup>
  import CheckboxConteiner from '../../../ui/sidebar/CheckboxConteiner.vue';
</script>
<template>
  <div class="filter-container">
    <div class="header">
      <h1>Бренд</h1>
      <span>Очистить</span>
    </div>
    <div class="search">
      <img src="@/images/Mobileicon.png" alt="" />
      <input type="text" placeholder="Поиск" />
    </div>
    <CheckboxConteiner />
  </div>
</template>
<style scoped>
.filter-container {
  margin-top: 28px;
  width: 100%;
  display: flex;
  flex-direction: column;
}
.search {
  margin-top: 16px;
  width: 100%;
  display: flex;
  align-items: center;
  height: 36px;
  border-radius: 4px;
  border: 1px solid #cbcbcb;
  padding: 10px 12px 10px 12px;
}
.search input {
  margin-left: 8px;
  width: 100%;
  outline: none;
  border: none;
  font-size: 14px;
  line-height: 16px;
  font-weight: 400;
  color: #aaaaaa;
}

.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.header h1 {
  font-size: 16px;
  line-height: 20px;
  font-weight: 700;
}
.header span {
  cursor: pointer;
  font-size: 12px;
  line-height: 12px;
  font-weight: 400;
  color: #aaaaaa;
  border-bottom: 1px solid #cbcbcb;
  transition: 0.5s ease-in;
}
.header span:hover {
  transition: 0.5s ease-in-out;
  border-bottom: 1px solid #7397f5;
  color: #7397f5;
}

</style>
