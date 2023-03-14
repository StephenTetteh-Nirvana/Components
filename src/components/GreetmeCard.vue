<template>
    <h2>Hello {{name}} and i like {{ hobby }}</h2>
</template>

<script>
    export default {
        name:'GreetmeCard',
        props:['name','hobby']
    }
</script>

<style scoped>

</style>