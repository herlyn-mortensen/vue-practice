<template>
    <div id="box"
    v-bind:style="{
        backgroundColor: color,
        }"
        ></div>
</template>


<script>

export default {
    data: function() {
        let theColor = randomColor();
        return {
            color: theColor,
        };
    },
};

function randomColor() {
    let color
    let numberColor = Math.floor(Math.random() * 3 + 1)
    if (numberColor > 1) {
        color = "red"
    } else if (numberColor > 2 ) {
        color = "blue"
    } else {
        color = "green"
    }
    return(color)
}

</script>

<style scoped>
#box {
 width: 50px;
 height: 50px;
 border: 1px solid black;
}
</style>
