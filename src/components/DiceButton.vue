<template>
    <div>
        <div class="even" v-if="number%2==0">
          <h1> {{ number }}! </h1>
        </div>
        <div class="odd" v-else>
          <h1> {{ number }} </h1>
        </div>
        <button @click="dice">Please click</button>
    </div>
</template>

<!-- 
  [x] step 1: Create a dice component.
  [x] step 2: When clicked on, will show a random number between 1 to 6.
  [x] step 3: Generate a random number in JavaScript using Math.random().
  [x] step 4: If the number is even, display an exclamation mark behind it (so 2!, 4!, 6!), 
  otherwise just display the number randomly.

 -->
<script>
//purpose is to hold the value of the randomNumber, to be produced on the 'dice' function.
let randomNumber = 0

export default {
  name: "DiceButton",  
  data: function () {
    return {
      number: randomNumber
    };
  },
  methods: {
    //must use 'this' to access variables inside the data object (line 26)
    dice: function() {
      randomNumber = Math.floor(Math.random() * 6 + 1)
      this.number = randomNumber
    },
  }

};

</script>


<style scoped>

</style>