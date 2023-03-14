<template>
    <ErrorPage>
        <h1 v-if="error.statusCode === 404" class="error-title">Page not found</h1>
        <h2 class="error-message">{{ error.message }}</h2>
    </ErrorPage>
</template>

<script>
    import ErrorPage from 'ui-app/src/components/ErrorPage.vue';
    export default{
        props:{
            error:{
                type: Object,
                required:true
            } 
        },
        layout: 'error',
        components:{
            ErrorPage
        }
    }
    // console.warn(typeof(error))
</script>