<template>
    <ListWrapper :header="header">
        <ListElement v-for="item in  menu" :key="item" :link="item.link" :title="item.title"/>
    </ListWrapper>
</template>

<script>
    import ListWrapper from "ui-app/src/components/ListWrapper.vue";
    import ListElement from "ui-app/src/components/ListElement.vue";
    export default{
        components:{
            ListWrapper, ListElement
        },
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