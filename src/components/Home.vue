<template>
    <div>
        <h1 v-on:mousemove="getConsole()">Home Component</h1>
        <button v-on:click="getData()">Click me</button>
        <button v-on:dblclick="getData('button double clicked')">Click me</button>
        <div>{{count}}</div>
    </div>
</template>

<script>
export default {
    name: 'HomE',
    data(){
        return {
            count : 0
        }
    },
    methods:{
        getData(data)
        {
            this.count = this.count+1;
        },
        getConsole(){
            console.warn("function colled");
        }
    }
};
</script>

<style scoped>
h1 {
    color: orange;
}
</style>
