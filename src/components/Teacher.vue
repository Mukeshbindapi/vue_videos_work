<template>
    <h1>Teacher Name is : {{ name }}</h1>
</template>

<script>
    export default {
        name : 'TeacheR',
        props: {
        name: {
            name: String,
        }
    }
    }
</script>