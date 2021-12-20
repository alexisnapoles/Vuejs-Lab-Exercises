<template>
  <div>
    <div @click="generateRandomNumber">{{ number }}</div>
  </div>
</template>

<script>
export default {
  data: function () {
    return {
      number: Math.floor(Math.random() * 6 + 1),
    };
  },
};
</script>

<style>
</style>