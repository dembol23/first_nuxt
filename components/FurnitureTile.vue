<template>
    <div class="furniture__tile">
        <slot></slot>
    </div>
</template>

<style lang="scss">
.furniture__tile{
    width: 45%;
    margin: 10px auto;
    display: flex;
    justify-content: center;
    align-items: center;
    font-size: 35px;
    padding: 70px 0;
    border-radius: 40px;
    background-color: #AED9ED;
    color: #fff;

    &:hover{
        background-color: #8ecae6;
        cursor: pointer;
    }
    svg{
        margin: 0 10px;
    }
}

</style>