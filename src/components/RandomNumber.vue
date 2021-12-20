<template>
  <!-- template serves as the "html"-ish area you see -->
  <!-- there should only be one root div or container for the whole component -->
  <div>
    <h1 class="random">{{ number }}</h1>
    <button v-on:click="getNewNumber">New Number</button>
  </div>
</template>

<script>
export default {
  // name refers to the current file name without the extension
  // name value should always have '' marks
  name: "RandomNumber",
  // data stores variables;
  data: function (e) {
    return {
      // without the button this changes via refresh
      number: Math.floor(Math.random() * 500 + 1),
    };
  },
  // ALL event handlers are stored in methods as per vue rules
  methods: {
    // there is duplicate in
    getNewNumber: function () {
      // 'this' refers to the data function
      this.number = Math.floor(Math.random() * 500 + 1);
    },
  },
};
</script>

<style scoped>
</style>