<script setup>
import {ref} from 'vue';

const Count = ref(0);

function increase () {
  Count.value++;
}

function decreese () {
  Count.value--;
}

</script>
<template>
  <main>
      <h1>Counter</h1>
      <span id="value">{{Count}}</span>
      <div>
        <button @click="decreese" id="decrement">-</button>
        <button @click="increase" id="decrement">+</button>
      </div>
    </main>
</template>

<style scoped>

main {
  text-align: center;
  background-color: #333;
  padding: 100px;
  border-radius: 20px;
}

#value {
  font-size: 50px;
}

button {
  font-size: 15px;
  margin: 0 5px;
  background-color: #555;
  color: #fff;
  cursor: pointer;
  border-radius: 4px;
}

button:hover {
  background-color: #777;
}

</style>