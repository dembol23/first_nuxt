<template>
    <div class="image-wrapper">
        <img :src="imageArray.src" class="image">
    </div>
</template>

<style>
    .image-wrapper{
        width: 50%;
        display: flex;
        justify-content: center;
        align-items: center;
    }
    .image{
        width: 100%;
        overflow: hidden;
    }
</style>

<script>
    export default{
        props:{
            imageArray:{
                type: Object,
                required: true
            }
        }
    }
</script>