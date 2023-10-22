<template>
  <div class="filter-container">
    <div class="filter">
      <div class="filter-title">
        <h1>Название категории</h1>
        <span>3</span>
      </div>
      <div class="filter-body">
        <div class="body">
          <h1>Название категории</h1>
          <span>3</span>
        </div>
        <div class="body">
          <h1>Название категории</h1>
          <span>3</span>
        </div>
        <div class="body">
          <h1>Название категории</h1>
          <span>3</span>
        </div>
      </div>
    </div>
  </div>
</template>
<style scoped>
.filter-container {
  width: 100%;
  align-items: center;
}
.filter {
  display: flex;
  flex-direction: column;
}
.filter h1 {
  color: #333333;
  font-weight: 400;
  font-size: 14px;
  line-height: 16px;
}
.filter span {
  color: #aaaaaa;
  font-weight: 400;
  font-size: 12px;
  line-height: 14px;
}
.filter-title {
  cursor: pointer;
  align-items: center;
  height: 30px;
  padding: 0px 16px 0px 8px;
  display: flex;
  justify-content: space-between;
  transition: .5s ease-in-out;
}
.filter-title:hover{
  background-color: #E2EFFF;
  border-radius: 5px;
  transition: .5s ease-in;
}
.filter-body {
  display: flex;
  flex-direction: column;
}

.body {
  cursor: pointer;
  height: 30px;
  padding: 0px 16px 0px 32px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  transition: .5s ease-in-out;
}
.body:hover{
  transition: .5s ease-in;
  background-color: #E2EFFF;
  border-radius: 5px;
}
</style>
