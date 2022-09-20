<template>
    <div>
        <h1 id="color" :style="{color:textColor}">
            {{result}}
        </h1>
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
        'textColor': 'green',
        };
    },
    methods: {
        addNumber: function(){
            this.result = resultNumber + 1;
            resultNumber = resultNumber + 1
            if (resultNumber%2 == 0) {
                this.textColor = 'green'
            } else {
                this.textColor = 'red'
            }
        },
        subtractNumber: function(){
            this.result = resultNumber - 1;
            resultNumber = resultNumber - 1
            if (resultNumber%2 == 0) {
                this.textColor = 'green'
            } else {
                this.textColor = 'red'
            }
        }
    },

}
</script>

<style scoped>

</style>