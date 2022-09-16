<template>
  <div>
    <h1 class="title">Vue welcomes you</h1>
    <h2>{{ message }}</h2>
    <button @click="changeMessage">Change Message</button>
    <button @click="toggleLight">Toggle Light</button>
    <div class="light" v-if="this.light==true">
        Lights On
    </div>
    <div class="light" v-else>
        Lights Off
    </div>
  </div>
</template>

<script>
export default {
  name: "Basic",
  data: function() {
    return {
      message: "Hello World",
      light:false
    };
  },
  methods: {
    changeMessage: function() {
      this.message = "Greetings People";
    },
    toggleLight: function() {
        this.light = !this.light;
    }
  }
};
</script>

<style scoped>
#box {
  border: 2px solid black;
}
</style>
