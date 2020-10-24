<template>
  <div class="hello">
    <h1>This is spencer</h1>
    <p>{{ number }}</p>
    <button @click="upper()">Press for 1</button>
  </div>
</template>

<script>

import {ref} from "vue"

export default {
  setup() {
    const number = ref(0)
    function upper(){
      number.value++
      }
      return {number, upper}
    },
  props: {
    msg: String
  }
}
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
