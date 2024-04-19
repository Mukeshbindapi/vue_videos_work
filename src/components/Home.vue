<template>
    <div>
        <h1>senr data child to parent in vue js 3</h1>
    </div>
    <h1>{{ childUser }}</h1>
    <User :getUser="getUserName" />
</template>

<script>
import User from './User.vue'
export default {
    name: 'HomE',
    components : {
        User
    },
    data(){
        return {
            childUser : ''
        }
    },
    methods : {
        getUserName(name){
            this.childUser = name
        }
    }
};
</script>

<style scoped>
h1 {
    color: orange;
}
</style>
