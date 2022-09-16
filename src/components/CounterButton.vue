<template>
    <div>
        <h1>{{result}}</h1>
        <button @click="addNumber">+</button>
        <button @click="subtractNumber">-</button>
    </div>

</template>

<script>
let resultNumber = 0;

export default {
    name: "CounterButton",
    data: function () {
        return {
        result: resultNumber,
        };
    },
    methods: {
        addNumber: function(){
            this.result = resultNumber + 1;
            resultNumber = resultNumber + 1
        },
        subtractNumber: function(){
            this.result = resultNumber - 1;
            resultNumber = resultNumber - 1
        }
    },

}
</script>

<style scoped>

</style>