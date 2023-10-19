<template>
  <div class="nav-container">
    <nav>
      <ui>
        <li>Информация о компании</li>
        <li>Контакты</li>
        <li>Полезные ссылки</li>
      </ui>
    </nav>
  </div>
</template>
<style scoped>
.nav-container {
  display: flex;
  height: 48px;
  align-items: center;
}
ui {
  display: flex;
  flex-direction: row;
  gap: 20px;
}
li {
  list-style: none;
  font-size: 14px;
  line-height: 16.94px;
  font-weight: 400;
  color: #393939;
  cursor: pointer;
  transition: 0.3s;
}
li:hover {
  color: #73aff4;
}
</style>
