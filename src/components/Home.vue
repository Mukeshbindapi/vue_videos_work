<template>
    <div>
        <h1 v-if="show">if condtion</h1>
        <h1 v-else>else condtion</h1>
        <button v-on:click="show=!show">toogle</button>
    </div>
</template>

<script>
export default {
    name: 'HomE',
    data(){
        return {
           show : false
        }
    }
};
</script>

<style scoped>
h1 {
    color: orange;
}
</style>
