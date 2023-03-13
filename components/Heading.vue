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
                if(this.level<1 || this.level>6){
                    return 'h1'
                }
                else{
                    return 'h' + this.level
                }
            }
        }
    }
</script>