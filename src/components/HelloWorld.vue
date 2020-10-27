<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <p>
      For a try and results on how to test with Jest on Vue.ts,<br />
      check out the
      <a href="https://tech.smartcamp.co.jp/" target="_blank" rel="noopener"
        >SMARTCAMP Engineer Blog</a
      >.
    </p>
    <h3>String Type Test</h3>
    <ul>
      <li>{{ string1 }}</li>
      <li>{{ string2 }}</li>
      <li>{{ string3 }}</li>
    </ul>
    <h3>Integer Type Test</h3>
    <ul>
      <li>{{ integer1 }}</li>
      <li>{{ integer2 }}</li>
      <li>{{ integer3 }}</li>
    </ul>
    <h3>Date Type Test</h3>
    <ul>
      <li>{{ date }}</li>
    </ul>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "HelloWorld",
  props: {
    msg: String
  },
  data() {
    return {
      string1: "babel",
      string2: "typescript",
      string3: "eslint",
      integer1: 111,
      integer2: 0,
      integer3: -111,
      date: new Date()
    };
  }
});
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
