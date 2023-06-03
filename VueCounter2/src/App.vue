<script setup>
import { ref } from "vue";
const count = ref(0);

const addToCount = () => {
  count.value++;
};

const subtractFromCount = () => {
  count.value--;
};
</script>

<!-- <script>
export default {
  data() {
    return {
      count: 0,
    };
  },
  methods: {
    addToCount() {
      this.count++;
    },
    subtractFromCount() {
      this.count--;
    },
  },
}; -->
<!-- </script> -->

<template>
  <main>
    <div>
      <h4>Current count is...</h4>
      <h1>{{ count }}</h1>
      <button @click="subtractFromCount()">-</button>
      <button @click="addToCount()">+</button>
    </div>
  </main>
</template>

<style scoped>
main {
  background-color: aliceblue;
  width: 100vw;
  height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
}

div {
  text-align: center;
}
</style>
