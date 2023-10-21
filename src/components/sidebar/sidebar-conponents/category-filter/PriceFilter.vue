<template>
  <div class="price-container">
    <div class="header">
      <h1>Цена</h1>
    </div>
    <div class="input-price">
      <div class="container-input">
        <span>от</span>
        <input type="text" value="5 500 ₽" />
      </div>
      <div class="line"></div>
      <div class="container-input">
        <span>до</span>
        <input type="text" value="6 500 ₽" />
      </div>
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
.container-input {
  display: flex;
  flex-direction: row;
  width: 119px;
  border-radius: 4px;
  border: 1px solid #d5d5d5;
  padding: 10px 8px 10px 8px;
  align-items: center;
}
input {
  margin-left: 6px;
  width: 100%;
  border: none;
  outline: none;
  font-size: 14px;
  line-height: 16px;
  font-weight: 400;
}
.container-input:focus {
  border: 1px solid #7397f5;
}

.line {
  margin: 0 16px;
  width: 10px;
  height: 1px;
  background-color: #d5d5d5;
}
</style>
