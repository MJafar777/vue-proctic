<template>
  <div>
    <h1>{{ count }}</h1>
    <button class="inc" v-on:click="increment">increment</button>
    <button class="dec" v-on:click="decrement">decrement</button>
    <button class="res" v-on:click="res">reset</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      count: 0,
    };
  },
  methods: {
    increment() {
      this.count += 1;
    },
    decrement() {
      this.count -= 1;
    },
    res() {
      this.count = 0;
    },
  },
};
</script>

<style scoped>
h1 {
  color: aqua;
}
.inc {
  background-color: green;
}
.dec {
  background-color: red;
}
* {
  cursor: pointer;
}
</style>
