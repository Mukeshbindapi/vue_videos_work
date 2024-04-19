<template>
    <div>
        <h1>Ref in vue js 3</h1>
        <input type="text" ref="first_input">
        <button @click="getData">Click me</button>
    </div>
</template>

<script>
export default {
    name: 'HomE',
    methods : {
        getData() {
            this.$refs.first_input.focus();
            let val = this.$refs.first_input.value;
            console.warn(val);
            this.$refs.first_input.style.color = 'red'
        }
    }
};
</script>

<style scoped>
h1 {
    color: orange;
}
</style>
