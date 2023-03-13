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
                required: true,
                min: 1,
                max: 6
            } 
        },
        computed:{
            headingLevel(){
                return 'h' + Math.min(Math.max(this.level,1),6)
            }
        }
    }
</script>