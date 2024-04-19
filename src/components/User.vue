<template>
    <div class="user">
        <h1>{{data.name}}</h1>
        <h2>{{ data.email }}</h2>
        <button v-on:click="getData(data.name)">Alert Name</button>
        <button v-on:click="getData(data.email)">Alert Email</button>
    </div>
   
</template>

<script>
    export default {
        name : 'UseR',
        props:{
            data : Object,
            getData : Function
        }
    }
</script>

<style>
.user{
    background-color: skyblue;
    padding: 10px;
    border-bottom: 1px solid;
    margin-bottom: 20px;

}
</style>