<template>
 <div id="app">
   <div id="message" :style="{color:textColor,fontSize:textSize}">
     Hello World</div>
     <button v-on:click="changeToRed">Red</button>
 </div>
</template>

<script>


export default {
 name: "App",
 data: function() {
  return {
    'textColor': 'green',
    'textSize': '32px',
  }
 },
 methods: {
  changeToRed:function(){
    this.textColor = 'red';
  }
 }
};
</script>

<style>
#app {

}
</style>