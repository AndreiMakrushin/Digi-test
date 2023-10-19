<script setup>
const props = defineProps({
  type: String,
  placeholder: String,
});
</script>

<template>
  <div class="search-container">
    <div class="container">
      <img class="search-icon" src="@/images/search.png" alt="" />
      <input
        :type="props.type"
        class="search-input"
        :placeholder="placeholder"
        @input="$emit('update:modelValue', $event.target.value)"
      />
    </div>
  </div>
</template>

<style scoped>
.search-container {
    width: 100%;
  height: 48px;
  border: 1px solid #73aff4;
  border-radius: 10px;
  display: flex;
  align-items: center;
  padding: 4px 16px;
}

.container {
  width: 100%;
  display: flex;
  align-items: center;
}

.search-icon {
  margin-right: 8px;
}
input{
  width: 100%;
}
input::marker {
    content: "\2660";
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
