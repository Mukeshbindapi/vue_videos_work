<template>
    <div>
        <h1>{{text}}</h1>
        <div v-html="tag"></div>
        <div v-html="tag2"></div>
    </div>
</template>

<script>
export default {
    name: 'HomE',
    data(){
        return {
            text : "Mukesh Bindra ji",
            tag : '<h1>Mukesh Kumar</h1>',
            tag2 : '<h2>mukesh@test.com</h2>'
        }
    }
};
</script>

<style scoped>
    h1 {
        color: orange;
    }
</style>
