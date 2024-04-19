<template>
    <div>
        <h1>Get input filed value</h1>
        <input type="text" placeholder="enter email" v-model="email"><br><br>
        <input type="text" placeholder="enter password" v-model="password"><br><br>
        <button v-on:click="getData()" type="button">Get Value</button>
    </div>
</template>

<script>
export default {
    name: 'HomE',
    data(){
        return {
            email : null,
            password : null
        }
    },
    methods : {
        getData(){
            console.warn("values :",this.email,this.password);
        }
    }
};
</script>

<style scoped>
h1 {
    color: orange;
}
</style>
