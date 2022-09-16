<template>
  <div>
    <h1>{{ message }}</h1>
    <button v-on:click="sayHi">Say Hi</button>
    <button v-on:click="editMessage">Say Goodbye</button>
    <button v-on:click="endMessage">Sleep</button>
  </div>
</template>
<script>
export default {
  name: "SayGreetings",
  data: function () {
    return {
      message: "Hi",
    };
  },
  methods: {
    sayHi: function () {
      this.message = "Hello World";
    },
    editMessage: function () {
      this.message = "Goodbye World";
    },
    endMessage: function () {
      this.message = "Zzzzz..zzzz";
    },
  },
};
</script>

<style scoped>
#box {
  border: 2px solid black;
}
</style>