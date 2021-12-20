<template>
  <div
    id="box"
    v-bind:style="{
      backgroundColor: color,
    }"
  ></div>
</template>

<script>
export default {
  data: function () {
    let colorsFinal = "";
    let colors = ["green", "red", "blue", "pink", "yellow"];
    let colorShow = Math.floor(Math.random() * 5);
    colorsFinal = colors[colorShow];
    return {
      color: colorsFinal,
    };
  },
};
</script>

<style>
#box {
  width: 50px;
  height: 50px;
  border: 1px solid whitesmoke;
}
</style>