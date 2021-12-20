<template>
  <div>
    <h1>{{ greetings }}</h1>
    <!-- 
    inline handler
    code eference: https://vuejs.org/v2/guide/events.html
     -->
    <button @click="say('Hello World')">Say Hi</button>
    <button @click="say('Goodbye World')">Say Goodbye</button>
    <button @click="say('zzz...zzz...zzz')">Sleep</button>
  </div>
</template>

<script>
export default {
  name: "SayGreetings",
  data: function () {
    return {
      greetings: "Say your greetings",
    };
  },
  methods: {
    say(message) {
      this.greetings = message;
    },
  },
};
</script>

<style scoped>
</style>