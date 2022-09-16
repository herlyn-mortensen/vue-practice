<template>
  <div id="app">
    <h1>Hello</h1>
    <Basic></Basic>
    <RandomBox></RandomBox>
    <RandomBox></RandomBox>
    <RandomBox></RandomBox>
    <SayGreetings></SayGreetings>
    <ColoredBox></ColoredBox>
    <CounterButton></CounterButton>
  </div>
</template>


<script>
import Basic from "./components/Basic";
import RandomBox from "./components/RandomBox";
import SayGreetings from "./components/SayGreetings";
import ColoredBox from "./components/ColoredBox";
import CounterButton from "./components/CounterButton";

export default {
  name: "App",
  components: {
    Basic,
    RandomBox,
    SayGreetings,
    ColoredBox,
    CounterButton,
  },
};
</script>

<style>
.title {
  font-family: Verdana;
}
</style>

