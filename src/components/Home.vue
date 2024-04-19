<template>
    <div>
        <h1>Reuse Component</h1>
        <ul>
            <li v-for="item in users" :key="item.name">
                <User :data="item" :getData="getData" />
            <</li>
        </ul>
    </div>
</template>

<script>
import User from './User.vue';
export default {
    name: 'HomE',
    components : {
        User
    },
    methods:{
        getData(name,email){
            alert(name,email)
        }
    },
    data(){
        return {
            users : [
                {
                    name : 'Mukesh Kumar',
                    email : 'mukesh123@gmail.com'
                },
                {
                    name : 'Ashish Kumar',
                    email : 'ashish123@gmail.com'
                },
                {
                    name : 'Jasavant Kumar',
                    email : 'jasavant123@gmail.com'
                },
                {
                    name : 'Himanshu Kumar',
                    email : 'himanshu123@gmail.com'
                },
                {
                    name : 'Jaihind Kumar',
                    email : 'jaihind123@gmail.com'
                }
            ]
        }
    }
};
</script>

<style scoped>
    h1 {
        color: orange;
    }
</style>
