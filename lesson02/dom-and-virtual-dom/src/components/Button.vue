<script lang="ts" setup>
import { ref } from "vue";

const count = ref(0);

function increment() {
  count.value++;
}
</script>

<template>
  <button id="count-button" aria-label="Click me" title="Count Button" @click="increment">
    Clicked {{ count }} times
  </button>
</template>

<style lang="css" scoped>
#count-button {
  background-color: #42b983;
  color: white;
  border: none;
  padding: 10px 20px;
  font-size: 16px;
  cursor: pointer;
  border-radius: 5px;
}
</style>
