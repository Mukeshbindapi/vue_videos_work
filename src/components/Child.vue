<template>
    <h1>{{name}}</h1>
    <h1>{{user.name}}</h1>
    <button v-on:click="getData()">call function</button>
</template>

<script>
    export default {
        name : 'ChilD',
        props : {
            name : String,
            user : Object,
            getData : Function
        }
    }
</script>