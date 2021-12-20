<template>
  <div id="app">
    <!-- there should always be an end tag -->
    <hr />
    Form
    <Form />

    <hr />
    Greet Someone Today
    <SayGreetings></SayGreetings>

    <hr />
    <OddEven></OddEven>

    <hr />
    Get Random Number
    <RandomNumber></RandomNumber>

    <hr />
    <ColorRandomizer></ColorRandomizer>
    <ColorRandomizer></ColorRandomizer>
    <ColorRandomizer></ColorRandomizer>
    <ColorRandomizer></ColorRandomizer>
  </div>
</template>


<script>
// importing the data from created component
import RandomNumber from "./components/RandomNumber";
import SayGreetings from "./components/SayGreetings";
import ColorRandomizer from "./components/ColorRandomizer";
import OddEven from "./components/OddEven";

// defines/identifies the component(s) to show on the template
export default {
  name: "App",
  components: {
    RandomNumber,
    SayGreetings,
    ColorRandomizer,
    OddEven,
  },
};
</script>

<style>
#app {
  font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
}
</style>
