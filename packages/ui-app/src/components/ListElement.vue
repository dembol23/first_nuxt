<template>
    <li>
        <nuxt-link :to="link" class="list-element">{{ title }}</nuxt-link>
    </li>
</template>

<style lang="scss" scoped>
    .list-element{
        text-decoration: none;
        color: #000;
        &:hover{
            text-decoration: underline;
        }
    }    
</style>

<script>
    export default{
        props:{
            title:{
                type: String,
                required: true
            },
            link:{
                type: String,
                required: true
            }
        }
    }
</script>