<template>
    <div>
        <h1>Two Way Binding</h1>
        <input type="text" v-model="count" />
        <h2>{{count}}</h2>
    </div>
</template>

<script>
export default {
    name: 'HomE',
    data(){
        return {
            count : 10
        }
    }
};
</script>

<style scoped>
h1 {
    color: orange;
}
</style>
