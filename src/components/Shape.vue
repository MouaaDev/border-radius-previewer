<template>
  <div class="rect"></div>
  <div class="inputs">
    <input type="text" />
    <input type="text" />
    <input type="text" />
    <input type="text" />
  </div>
</template>

<script>
export default {}
</script>

<style>
.rect {
  width: 400px;
  height: 400px;
  background-color: #dfc155;
  margin-bottom: 2rem;
}

.inputs {
  display: flex;
  align-items: center;
  justify-content: center;
}

.inputs input {
  width: 80px;
  margin-left: 1rem;
  text-align: center;
  font-family: inherit;
  padding: 0.2rem;
}

.inputs input:first-child {
  margin: 0;
}
</style>
