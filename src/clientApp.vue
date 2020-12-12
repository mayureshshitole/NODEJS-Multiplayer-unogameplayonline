<template>
    <div>
        <UnoGame :socket="socket"></UnoGame>
    </div>
</template>

<script>

    import socket from 'socket.io-client'    
    import UnoGame from "./UnoGame"

    export default {
        name: "clientApp",
        data: function() {
            return {               
                socket: socket("https://uno-game-mayu.herokuapp.com/:" + 3000),
            }
        },
        components: {
            UnoGame
        },
    }
</script>

<style scoped>

</style>

<style>
    body {
        background: #90c060;
        margin:0 auto;
        width:100%;
        font: 12px normal Verdana, Arial, Helvetica, sans-serif;
        user-select: none;
        overflow: hidden;
        transform: scale(1.0);
    }
    a{
        text-decoration:none;
        color:inherit;
    }

</style>