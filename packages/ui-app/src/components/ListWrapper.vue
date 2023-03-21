<template>
    <div class="list-wrapper">
        <h2 class="list-title">{{ header }}</h2>
        <ul class="list">
            <slot></slot>
        </ul>
    </div>
</template>
<style lang="scss" scoped>
    .list{
        list-style-type: '- ';
        font-size: 1.9rem;
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
        &-title{
            font-size: 2.3rem;
            text-decoration: underline;
        }
        &-wrapper{
            margin: auto;
            width: 70%;
            display: flex;
            justify-content: center;
            align-items: center;
            flex-direction: column;
        }
    }
    
</style>
<script>
    export default{
        props:{
            header:{
                type: String,
                required: true
            },
            menu:{
                type: Array,
                required: true
            }
        }
    }
</script>