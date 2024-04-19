<template>
    <div>
        <h1>for loop in vue js </h1>
        <ul>
            <li v-for="item in technology" :key="item">{{ item }}</li>
        </ul>
        <br><br>
        <ul>
            <li v-for="item in user" :key="item.email">
                Name is : {{ item.name }} and email is : {{ item.email }}
            </li>
        </ul>
    </div>
</template>

<script>
export default {
    name: 'HomE',
    data(){
        return {
            technology : ['java','php','node','html'],
            user : 
            [
                {
                    name : 'mukesh kumar',
                    email : 'mukesh@gmail.com'
                },
                {
                    name : 'ashish kumar',
                    email : 'ashish@gmail.com'
                },
                {
                    name : 'jasavant kumar',
                    email : 'jasavant@gmail.com'
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
