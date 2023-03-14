<template>
    <div>
        <slot></slot>
    </div>
</template>

<style lang="scss" scoped>
    .error{
        &-title{
            text-align: center;
            margin-top: 100px;
            font-size: 4rem;
        }
        &-message{
            text-align: center;
            margin-top: 100px;
            font-size: 3rem;
        }
    }
</style>