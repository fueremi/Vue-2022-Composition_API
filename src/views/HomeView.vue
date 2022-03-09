<script setup>
import { ref } from "vue";

const counter = ref(0);

const increaseCounter = () => counter.value++;
const decreaseCounter = () => counter.value--;
</script>

<template>
  <main>
    <h1>Home</h1>

    <h3>Counter</h3>
    <button class="button" @click="decreaseCounter">-</button>
    <span>{{ counter }}</span>
    <button class="button" @click="increaseCounter">+</button>
  </main>
</template>

<style scoped>
h1 {
  margin-bottom: 0.7rem;
}
h3 {
  margin-bottom: 10px;
}
.button {
  border: 1px solid #ebebeb;
  background: #fff;
  border-radius: 5px;
  padding: 8px 16px;
}
span {
  margin: 0 16px;
  font-size: 1.3rem;
  color: hsla(160, 100%, 37%, 1);
}
</style>
