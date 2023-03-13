<template>
    <span :v-html="headingLevel">
        <slot></slot>
    </span>
</template>
<script>
    export default{
        props:{
            level:{
                type: Number,
                required: true
            } 
        },
        computed:{
            headingLevel(){
                return 'h' + this.level
            }
        }
    }
</script>