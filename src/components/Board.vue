<template>
    <div class="table">
        <div class="grad"></div>
       <div>If anyone leave the game then game will stop for every player</div>
        <slot></slot>
    </div>

    
</template>


<script>
    export default {
        name: "Board"
    }
</script>

<style scoped>
    .table{
        position:absolute;
        width:100%;
        height:80%;        
        border-bottom:solid 3px #FFFF00;
        border-top:solid 3px #008000;
        border-left:solid 3px #FF0000;
        border-right:solid 3px #0000FF;
        border-radius:15px;
        background:url('../../public/img/table.jpg')no-repeat;
        background-repeat: round;
        box-shadow:0 6px 15px rgb(75, 72, 72);
        transform-style: preserve-3d;
       
    }
   /* .grad{
        position:relative;
        width:100%;
        height:100px;
        background:url('../../public/img/bg_grad.png')no-repeat;
        background-repeat: round;
    }*/
</style>