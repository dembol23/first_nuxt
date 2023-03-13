<template>
    <div>
        <h1 v-if="error.statusCode === 404" class="error-title">Page not found</h1>
        <h2 class="error-message">{{ error.message }}</h2>
        <Heading :level="1">asasas</Heading>
    </div>
</template>

<style lang="scss" scoped>
    .error{
        &-title{
            text-align: center;
            margin-top: 100px;
            font-size: 4rem;
        }
        &-message{
            text-align: center;
            margin-top: 100px;
            font-size: 3rem;
        }
    }
    h1{
        color: red;
    }
</style>

<script>
    export default{
        props : ['error'],
        layout: 'error'
    }
</script>