<template>
  <h1 class="header">
    <i class="fas fa-border-style"></i>
    Border Radius Previewer
  </h1>
  <Shape />
  <SourceCode />
</template>

<script>
import Shape from "./components/Shape.vue"
import SourceCode from "./components/SourceCode.vue"

export default {
  components: {
    Shape,
    SourceCode,
  },
}
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Poppins:wght@600;700&family=Source+Code+Pro:wght@700&display=swap");

*,
*::before,
*::after {
  box-sizing: border-box;
}

body {
  margin: 0;
  font-family: "Poppins", sans-serif;
  background-color: #232323;
  min-height: 100vh;
  height: 150vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: flex-start;
}

#app {
  max-width: 800px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}

.header {
  font-size: 2.5rem;
  background: linear-gradient(270deg, #d6b33a 0%, #d14141 100%);
  background-clip: text;
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  margin: 1.5rem 0 1.5rem 0;
}
</style>
