<template>
  <div class="source-code">
    <h2>Source Code:</h2>
    <pre><code><em>border-top-left-radius:</em> 0;
<em>border-top-right-radius:</em> 0;
<em>border-bottom-right-radius:</em> 0;
<em>border-bottom-left-radius:</em> 0;

<em class="comment">/* Shorthand Syntax */</em>
<em>border-radius:</em> 0;
    </code></pre>
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
.source-code {
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  color: #fff;
  margin-top: 2.5rem;
}

.source-code h2 {
  margin-bottom: 0;
}

.source-code code {
  display: inline-block;
  font-family: "Source Code Pro", sans-serif;
  background-color: #4d4d4d;
  width: 400px;
  padding: 1rem;
  margin-top: 0.1rem;
  border-radius: 10px;
  color: #d6b33a;
}

.source-code em {
  color: #45bcd6;
  font-style: normal;
}

.source-code em.comment {
  color: #969696;
  font-style: normal;
}
</style>
