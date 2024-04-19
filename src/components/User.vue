<template>
    <h1>User component</h1>
    <button @click="getUser(UserName)">Send User Name</button>
</template>

<script>
    export default {
        name : 'UseR',
        data(){
            return {
                UserName : "Mukesh Kumar"
            }
        },
        props:{
            getUser : Function
        }
    }
</script>