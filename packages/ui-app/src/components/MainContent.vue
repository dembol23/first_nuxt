<template>
    <main class="main">
        <Navigation />
        <div class="content">
            <slot></slot>
        </div>
    </main>
</template>

<style scoped>
.main{
    margin: 0;
    width: 100%;
    height: 100%;
}
.content{
    width: 100%;
}
</style> 

<script>
    import Navigation from 'ui-app/src/components/Navigation.vue';
    export default{
        components:{
            Navigation
        }
    }
</script>