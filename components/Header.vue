<template>
<div>
    <div class="TopHeader">
    </div>
    <div class="Header">
    <img class="logo" src="../assets/img/logo.png" />
    <nav tag="h1" class="mb-1">DAY BETTER YOU</nav>
    <div class="menu">
    <a class="home" href="">หน้าแรก</a>
    <a class="program" href="#">โปรแกรม</a>
    <a class="contact" href="#">ติดต่อเรา</a>
    <div class="button">
    <Button class="bt-begin">เริ่มโปรแกรม</Button>
    </div>
    </div>
</div>
</div>
</template>
<style lang="scss" >
@import '../styles/vars/color' ;
@import '../styles/vars/font' ;

  .TopHeader{
    position: absolute;
    width: 100%;
    bottom: 94.12%;
    background: $main-color;
    }
    .Header{
    position: absolute;
    color: #000000;
    background: #ffffff;
    height: 64px;
    width: 100%;
    left: 0px;
    top: 4px;
    border-radius: 0px;
    }
    .logo{
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    position: absolute;
    height: 32px;
    width: 32px;
    border-radius: 0px;
    top: 19px;
    margin-left:  56px;
    }
    .mb-1{
    position: absolute;
    height: 26px;
    left: 94px;
    top: 23px;
    font-family: $main-font;
    font-size: 20px;
    font-style: normal;
    font-weight: 700;
    line-height: 26px;
    letter-spacing: 0px;
    text-align: left;
    color: $main-color;
    }
    .menu {
    position: relative;
    float:       right;
}
.menu a{
    padding-top: 23px;
    list-style: none;
    display: inline-block;
    color: #000000;
    font-weight: 400;
    margin-left: 40px;
    text-decoration: none;
}
.button{
    margin-left:  65px;
    margin-right: 56px;
    float:       right;
    position: relative;
    padding-top:  10px;
}

    </style>