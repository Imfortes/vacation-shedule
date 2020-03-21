<template>
    <div class="menu">
        <a href="#" class="menu-link active">Dashboard</a>
        <a href="#" class="menu-link">Team line up</a>
    </div>
</template>

<script>
    export default {

    }
</script>

<style scoped>
    .menu{
        width: 90vw;
        height: 57px;
        margin: 0 auto;
        background: #f7f7f7;
        display: flex;
        flex-direction: row;
        align-items: center;
    }
    .menu-link{
        border-radius: 2px;
        padding: 12px 73px;
        font-size: 14px;
        color: #CACACA;
        text-align: center;
        line-height: 12px;
        margin-left: 20px;
        margin-right: 20px;
        transition: .5s;
        text-decoration: none;
    }
    .menu-link:not(.active){
        background: #fff;
        margin-right: 0;
        margin-left: 0;
    }
    .active,
    .menu-link:hover{
         background: #556080;
    }
</style>