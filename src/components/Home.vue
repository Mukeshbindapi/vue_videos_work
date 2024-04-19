<template>
    <h1>Email : {{email}}</h1>
    <h1>Mobile : {{mobile}}</h1>
    <h1>Name : {{getName('mukesh')}}</h1>
</template>

<script>
    export default {
        name : 'HomE',
        data(){
            return {
                email : 'mukesh@gmail.com',
                mobile : '2345617895',
                getName:function(a){
                    return a;
                }
            }
        }
    }
</script>

<style scoped>
    h1{
        color: orange;
    }
</style>