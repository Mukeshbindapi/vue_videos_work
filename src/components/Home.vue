<template>
    <div>
        <h1>Pass data to Child Component</h1>
    </div>
    <Child name="Mukesh Kumar" :user="user" :getData="getData" />
</template>

<script>
import Child from './Child.vue'
export default {
    name: 'HomE',
    components : {
        Child
    },
    data()
    {
        return {
            user : {name : 'mukesh kumar', email : 'mukeshbindra@gmail.com'}
        }
    },
    methods : {
        getData(){
            console.warn("function colled");
            alert("Hellow")
        }
    }
};
</script>

<style scoped>
    h1 {
        color: orange;
    }
</style>
