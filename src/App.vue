<template>
  <div id="app">
    <StyleBinding></StyleBinding>
    <hr>
    <DiceButton></DiceButton>
    <hr>
    <CounterButton></CounterButton>
    <hr>
    <ColoredBox></ColoredBox>
    <hr>
    <SayGreetings></SayGreetings>
    <hr>
    <RandomBox></RandomBox>
    <RandomBox></RandomBox>
    <RandomBox></RandomBox>
    <h1>Hello</h1>
    <hr>
    <Basic></Basic>
  </div>
</template>


<script>
import Basic from "./components/Basic";
import RandomBox from "./components/RandomBox";
import SayGreetings from "./components/SayGreetings";
import ColoredBox from "./components/ColoredBox";
import CounterButton from "./components/CounterButton";
import DiceButton from "./components/DiceButton";
import StyleBinding from "./components/StyleBinding";

export default {
  name: "App",
  components: {
    Basic,
    RandomBox,
    SayGreetings,
    ColoredBox,
    CounterButton,
    DiceButton,
    StyleBinding,
  },
};
</script>

<style>
.title {
  font-family: Verdana;
}
</style>

