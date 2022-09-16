<template>
  <div id="box">{{ number }}</div>
</template>
<script>
export default {
  data: function () {
    return {
      number: Math.floor(Math.random() * 100 + 1),
    };
  },
};
</script>
<style scoped>
#box {
  border: 2px solid black;
}
</style>