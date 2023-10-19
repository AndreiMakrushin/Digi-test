<script setup>
const props = defineProps({
  text: String,
});
</script>

<template>
  <div class="button">
    <button>{{ props.text }}</button>
  </div>
</template>
<style scoped>
.button {
  display: flex;
}

button {
  outline: #73aff4;
  width: 108px;
  height: 48px;
  padding: 8px 24px;
  border: 1px solid #73aff4;
  border-radius: 8px;
  font-size: 14px;
  line-height: 16.94px;
  font-weight: 500;
  cursor: pointer;
  transition: transform 0.2s;
  transition: 0.6s ease;
  background-color: transparent;
}

button:active {
  transform: scale(0.95);
}
button:hover {
  background-color: #73aff4;
  color: #fff;
}
</style>
