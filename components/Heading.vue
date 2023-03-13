<template>
    <component :is="headingLevel">
        <slot></slot>
    </component>
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