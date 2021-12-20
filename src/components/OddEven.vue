<template>
  <div>
    <div class="counter">{{ count }}</div>
    <div style="color: green" v-if="this.count % 2 === 0">Even</div>
    <div style="color: orange" v-else>Odd</div>

    <button @click="increment">+</button>
    <button @click="decrement">-</button>
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
    increment: function () {
      this.count++;
    },
    decrement: function () {
      this.count--;
    },
  },
};
</script>

<style>
.counter {
  border: 1px solid black;
  display: flex;
  justify-content: center;
  align-items: center;
  width: 50px;
  height: 50px;
}
.odd {
  color: orange;
}
.even {
  color: green;
}
</style>