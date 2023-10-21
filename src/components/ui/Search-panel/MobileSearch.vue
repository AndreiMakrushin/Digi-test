<script setup>
const props = defineProps({
  type: String,
  placeholder: String,
});
</script>

<template>
  <div class="search-container-mobile">
    <div class="container-mobile">
      <img class="search-icon-mobile" src="@/images/back.png" alt="" />
      <input
        :type="props.type"
        class="search-input"
        :placeholder="placeholder"
        @input="$emit('update:modelValue', $event.target.value)"
      />
      <img class="search-icon-mobile-clear" src="@/images/close.png" alt="" />
      
    </div>
  </div>
</template>

<style scoped>
.search-container-mobile {
  width: 100%;
  height: 48px;
  border-radius: 10px;
  display: flex;
  align-items: center;
  padding: 4px 8px;
  margin-right: 8px;
}

.container-mobile {
  border-bottom: #d5d5d5;
  width: 100%;
  display: flex;
  align-items: center;
}

.search-icon-mobile {
  margin-right: 8px;
}
.search-icon-mobile-clear{
    color: black;
}
input {
  width: 100%;
}
.search-input {
  display: flex;
  font-size: 16px;
  font-weight: 400;
  line-height: 24px;
  flex: 1;
  border: none;
  outline: none;
  background-color: transparent;
}
</style>
