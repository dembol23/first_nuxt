<template>
    <MediaWrapper>
        <TextWrapper :textArray="textArray" />
        <ImageWrapper :imageArray="imageArray" />
    </MediaWrapper>
</template>

<script>
    import MediaWrapper from "ui-app/src/components/MediaWrapper.vue";
    import TextWrapper from "ui-app/src/components/TextWrapper.vue";
    import ImageWrapper from "ui-app/src/components/ImageWrapper.vue";
    export default{
        components:{
            MediaWrapper, TextWrapper, ImageWrapper
        },
        props:{
            header:{
                type: String,
                required: true
            },
            subheader:{
                type: String,
                required: true
            },
            bodytext:{
                type: String,
                required: true
            },
            gallery:{
                type: Object,
                required: true
            }
        },
        computed:{
            textArray(){
                const textArray = {'header':this.header,'subheader':this.subheader,'text':this.bodytext}
                return textArray
            },
            imageArray(){
                const imageArray = {'src':this.gallery.rows['1'].columns['1'].publicUrl,'height':this.gallery.rows['1'].columns['1'].properties.dimensions.height,'width':this.gallery.rows['1'].columns['1'].properties.dimensions.width}
                return imageArray
            }
        }
    }
</script>