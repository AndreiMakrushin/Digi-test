<script setup>
import ButtonCard from "@/components/ui/buttons/ButtonCard.vue";
</script>

<template>

    <div class="card">
      <div class="header">
        <div class="hit">
          <h1>Хит продаж</h1>
          <img src="@/images/fire.png" alt="" />
        </div>
        <div class="kubik">
          <img src="@/images/kubik.png" alt="" />
        </div>
        <div class="sale">
          <span>25%</span>
        </div>
      </div>
      <div class="brand">
        <h1>Бренд</h1>
        <p>
          Полное название товара в несколько строк для вида с обрывом в конце...
        </p>
      </div>

      <div class="price">
        <span class="current-price">5 990 ₽</span>
        <span class="old-price">5 990 ₽</span>
      </div>
      <ButtonCard />
    </div>
  
</template>

<style scoped>

.card {
  max-width: 333px;
  display: flex;
  flex-direction: column;
  width: 100%;
}
.header {
  background-repeat: no-repeat;
  background-size: cover;
  flex-direction: column;
  background-color: #f8f8fa;
  height: 200px;
}
.hit {
  margin-left: 12px;
  margin-top: 12px;
  margin-right: 12px;
  position: relative;
  background-color: #fff;
  max-width: 112px;
  height: 32px;
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  border-radius: 4px;
  border: 1px solid#F2F2F2;
}
.hit h1 {
  margin-right: 4px;
  font-size: 14px;
  line-height: 16px;
  font-weight: 400;
}
.sale {
  margin-left: 12px;
  display: flex;
  width: 48px;
  height: 26px;
  border-radius: 4px;
  background-color: #7397f5;
  padding: 6px 10px 6px 10px;
  color: #ffffff;
  justify-content: center;
  align-items: center;
  cursor: pointer;
  transition: 0.3s ease-in;
}
.sale:hover {
  transition: 0.3s ease-in-out;
  scale: 1.2;
}
.sale span {
  font-weight: 700;
  font-size: 14px;
  line-height: 14px;
}
.kubik {
  padding: 27px 0px 27px 0px;
  text-align: center;
}
.brand {
  margin-top: 16px;
}
.brand h1 {
  font-weight: 400;
  font-size: 14px;
  line-height: 16px;
  color: #aaaaaa;
}
.brand p {
  margin-top: 8px;
  font-weight: 400;
  font-size: 14px;
  line-height: 16px;
  color: #333333;
}
.price {
  margin-top: 16px;
}
.price .old-price {
  text-decoration: line-through;
  margin-left: 8px;
  font-weight: 400;
  font-size: 12px;
  line-height: 14px;
  color: #aaaaaa;
}
.current-price {
  color: #333333;
  font-weight: 700;
  font-size: 16px;
  line-height: 14px;
}
</style>
