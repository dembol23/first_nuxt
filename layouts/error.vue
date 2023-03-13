<template>
    <div>
        <h1 v-if="error.statusCode === 404" class="error-title">Page not found</h1>
    </div>
</template>

<style lang="scss" scoped>
    .error-title{
        text-align: center;
        margin-top: 100px;
    }
</style>

<script>
    export default{
        props : ['error'],
        layout: 'error'
    }
</script>