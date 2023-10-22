<script setup>
    const props = defineProps({
    span: String,
    value: Number
  })
</script>
<template>
  <div class="container-input">
    <span>{{ props.span }}</span>
    <input type="text" :value="props.value + ' ₽'" />
  </div>
</template>
<style scoped>
.container-input {
  display: flex;
  flex-direction: row;
  width: 119px;
  border-radius: 4px;
  border: 1px solid #d5d5d5;
  padding: 10px 8px 10px 8px;
  align-items: center;
}
span {
  font-size: 12px;
  line-height: 14px;
  color: #aaaaaa;
  font-weight: 400;
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
</style>
