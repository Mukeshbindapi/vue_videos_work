<template>
    <div>
        <h1>Get Check box & redio button value</h1>
        <h3>technology</h3>
        <label for="java">java</label>
        <input type="checkbox" value="java" id="java" v-model="technology">

        <label for="php">php</label>
        <input type="checkbox" value="php" id="php" v-model="technology">

        <label for="node">node</label>
        <input type="checkbox" value="node" id="node" v-model="technology">
        <br><br>

        <h3>who i am</h3>
        <label for="student">student</label>
        <input type="radio" value="student" v-model="who" name="who" id="student">

        <label for="developer">developer</label>
        <input type="radio" value="developer" v-model="who" name="who" id="developer">
        <br><br>
        <h4>select technology : {{ technology }}</h4>
        <h4>I am a : {{ who }}</h4>
    </div>
</template>

<script>
export default {
    name: 'HomE',
    data(){
        return {
            technology : [],
            who : null
        }
    }
};
</script>

<style scoped>
h1 {
    color: orange;
}
</style>
