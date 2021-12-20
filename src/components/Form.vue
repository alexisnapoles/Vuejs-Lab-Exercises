<template>
  <div>
    <form>
      <div>
        <label>First Name</label>
        <input type="text" v-model="first_name" />
      </div>
    </form>
    <div>
      <h1>Your details</h1>
      <ul>
        <li>First Name: {{ first_name }}</li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  data: function () {
    return {
      first_name: "",
    };
  },
};
</script>