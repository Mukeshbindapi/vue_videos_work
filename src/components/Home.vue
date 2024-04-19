<template>
    <div>
        <h1>CSS Binding</h1>
        <h2 :class="ApplyStyle">Home Component</h2>
        <button @click="colorfull = !colorfull">Apply Style</button>
    </div>
</template>

<script>
export default {
    name: 'Home',
    data() {
        return {
           colorfull: true,
        }
    },
    computed: {
        ApplyStyle() {
            return {
                test: this.colorfull,
                test1: true,
                other: true
            }
        }
    }
};
</script>

<style scoped>
h1 {
    color: orange;
}

.test {
    background-color: green;
    width: 200px;
    padding: 10px;
    text-align: center;
    margin-left: 42%;
    color: #fff;
}

.test1 {
    color: red;
    width: 200px;
    padding: 10px;
    text-align: center;
    margin-left: 42%;
}

.other {
    font-size: 50px;
}
</style>
