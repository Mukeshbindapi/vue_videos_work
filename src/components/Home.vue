<template>
    <div>
        <h1>Props in Vue.js 3</h1>
        <Student :name="name" />
        <Teacher :name="name" />
    </div>
</template>

<script>
import Student from './Student.vue';
import Teacher from './Teacher.vue';

export default {
    name: 'HomE',
    components: {
        Student,
        Teacher
    },
    data(){
        return {
            name : 'Who ore you'
        }
    }
};
</script>

<style scoped>
h1 {
    color: orange;
}
</style>
