<template>
    <div class="text-wrapper">
        <h2 class="text-header">{{ textArray.header }}</h2>
        <h4 class="text-subheader">{{ textArray.subheader }}</h4>
        <p v-html="textArray.text" class="text"></p>
    </div>
</template>

<style lang="scss" scoped>
    .text{
        font-size: 1.6rem;
        &-wrapper{
            width: 50%;
        }
        &-subheader{
            font-size: 1.9rem;
        }
        &-header{
            font-size: 2.3rem;
            text-decoration: underline;
        }
    }
</style>

<script>
    export default{
        props:{
            textArray:{
                type: Object,
                required: true
            }
        }
    }
</script>