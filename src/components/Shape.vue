<template>
  <div
    :style="{
      borderRadius: `${topLeftRadius}px ${topRightRadius}px ${bottomRightRadius}px ${bottomLeftRadius}px `,
    }"
    class="rect"
  ></div>
  <div class="inputs">
    <input type="text" v-model="topLeftRadius" />
    <input type="text" v-model="topRightRadius" />
    <input type="text" v-model="bottomRightRadius" />
    <input type="text" v-model="bottomLeftRadius" />
  </div>
  <SourceCode
    :topLeft="topLeftRadius"
    :topRight="topRightRadius"
    :bottomRight="bottomRightRadius"
    :bottomLeft="bottomLeftRadius"
  />
</template>

<script>
import SourceCode from "./SourceCode.vue"

export default {
  components: { SourceCode },
  data() {
    return {
      topLeftRadius: 0,
      topRightRadius: 0,
      bottomRightRadius: 0,
      bottomLeftRadius: 0,
    }
  },
}
</script>

<style scoped>
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

@media screen and (max-width: 674px) {
  .rect {
    width: 250px;
    height: 250px;
  }
}
</style>
