<template>
  <div class="checkbox-container">
    <label class="checkbox">
      <div class="input-container">
        <input type="checkbox" name="checkbox" />
        <h1>Атрибут</h1>
      </div>
      <span>3</span>
    </label>

    <label class="checkbox">
      <div class="input-container">
        <input type="checkbox" name="checkbox" />
        <h1>Атрибут</h1>
      </div>
      <span>3</span>
    </label>

    <label class="checkbox">
      <div class="input-container">
        <input type="checkbox" name="checkbox" />
        <h1>Атрибут</h1>
      </div>
      <span>3</span>
    </label>

    <label class="checkbox">
      <div class="input-container">
        <input type="checkbox" name="checkbox" />
        <h1>Атрибут</h1>
      </div>
      <span>3</span>
    </label>

    <label class="checkbox">
      <div class="input-container">
        <input type="checkbox" name="checkbox" />
        <h1>Атрибут</h1>
      </div>
      <span>3</span>
    </label>

    <label class="checkbox">
      <div class="input-container">
        <input type="checkbox" name="checkbox" />
        <h1>Атрибут</h1>
      </div>
      <span>3</span>
    </label>
  </div>
</template>
<style scoped>
.checkbox-container {
  height: 180px;
  width: 100%;
  margin-top: 20px;
  overflow: auto;
  scrollbar-color: #cbcbcb;
}
.checkbox-container::-webkit-scrollbar {
  background-color: transparent;
  width: 1px;
}
.checkbox-container::-webkit-scrollbar-thumb {
  background-color: #cbcbcb;
}
.checkbox {
  cursor: pointer;
  width: 100%;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
  padding: 0px 16px 0px 0px;
  margin-bottom: 12px;
}

.input-container {
  display: flex;
  flex-direction: row;
  align-items: center;
}
.input-container input {
  width: 20px;
  height: 20px;
  border-radius: 3px;
  border: 1px solid #7397f5;
}
.input-container h1 {
  margin-left: 12px;
  color: #333333;
  font-weight: 400;
  font-size: 14px;
  line-height: 16px;
}
.checkbox span {
  color: #aaaaaa;
  font-weight: 400;
  font-size: 12px;
  line-height: 14px;
}
</style>
