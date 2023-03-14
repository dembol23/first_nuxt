<template>
    <div class="furniture-list">
        <slot></slot>
    </div>
</template>

<style lang="scss" scoped>
.furniture-list{
    width: 80%;
    margin:10px 10%;
    height: auto;
    display: flex;
    flex-wrap: wrap;
}
</style>