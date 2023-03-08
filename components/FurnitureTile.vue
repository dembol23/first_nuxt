<template>
    <div class="furniture-types__tile">
        <slot></slot>
    </div>
</template>
<style scoped>
.furniture-types__tile{
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
}
.furniture-types__tile:hover{
    background-color: #8ecae6;
    cursor: pointer;
}
.furniture-types__tile *{
    margin: 0 10px;
}
</style>