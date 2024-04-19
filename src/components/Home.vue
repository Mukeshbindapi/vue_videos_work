<template>
    <div>
        <h1>Email: {{ email }}</h1>
        <h1>Name: {{ getName('Mukesh') }}</h1>
        <h1>All Data: {{ getData().email }}</h1>
    </div>
</template>

<script>
export default {
    name: 'Home',
    data() {
        return {
            email: 'mukesh@gmail.com',
        };
    },
    methods: {
        getName(name) {
            return name;
        },
        getData() {
            return {
                name: 'Mukesh Kumar',
                email: this.email,
            };
        },
    },
};
</script>

<style scoped>
h1 {
    color: orange;
}
</style>
