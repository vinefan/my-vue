<template>
    <div id="header">
    <div id="logo"><i class="el-icon-s-tools"></i><div>善行保</div></div>
    <div id="menu">
        <a  href="#"
            v-on:onmouseenter="changeColor" 
            v-bind:class="insure-link">
            <i class="el-icon-tickets"> 投保</i>
        </a> |
        <a  href="#"
            v-on:on>
            <i class="el-icon-paperclip"> 申述</i>
        </a> |
        <a class="vote-link" href="#">
            <i class="el-icon-edit-outline"> 投票</i>
        </a>
    </div>
    </div>
</template>

<script>
    export default {
        name: "Header",
        data: function () {
            return {
                onColor : "#333",
                offColor : "#456789",
                isOver: 0
            }
        },
        methods:{
            changeColor: function (){
                
            }
        }
    }
</script>

<style scoped>
    #header{
        height: 90px;
        background-color: #eeeeee 
    }
    #logo{
        width: 275px;
        height: 90px;
        display: inline-block;
        color:steelblue;
    }
    #logo i {
        margin-top: 25px;
        font-size: 40px;
        height: 100px;
        display: inline-block;
        
    }
    #logo div{
        margin-left: 20px;
        font-size: 40px;
        display: inline-block;
    }
    #menu{
        display: inline-block;
        font-size: 22px;
        width: 300px;
        height: 90%;
        margin-left: 40%
    }

    #menu a{
        color: #333;
        display: inline-block;
        width: 80px;
    }
    

</style>
