
<template>
  <div class="sell-batton">
    <button>Купить</button>
  </div>
</template>
<style scoped>
.sell-batton {
  display: flex;
  width: 100%;
  justify-content: flex-start;
}
button {
  cursor: pointer;
  height: 38px;
  border-radius: 4px;
  border: 1px solid #7397f5;
  padding: 12px 16px 12px 16px;
  margin-top: 16px;
  font-weight: 700;
  font-size: 14px;
  line-height: 14px;
  background: #ffffff;
  text-align: center;
  color: #7397f5;
  transition: 0.3s ease-in;
}
button:hover {
  transition: 0.3s ease-in-out;
  background-color: #7397f5;
  color: #ffffff;
}
</style>
