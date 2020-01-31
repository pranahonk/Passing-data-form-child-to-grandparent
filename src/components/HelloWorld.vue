<template>
  <div class="hello">
    <h1>{{ Message }}</h1>
    <Hello :msg="message2"/>
    <button>Hello</button>
  </div>
</template>

<script>
import Hello from "./Hello";
export default {
  name: "HelloWorld",
  components: {
    Hello: Hello
  },
  props: {
    Message: {
      type: String,
      default: "Keren cuy"
    },
    message2: {
      type: String,
      default: "Keren cuy"
    }
  }
};
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
