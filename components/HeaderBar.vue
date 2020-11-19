<template>
<div>
    <div class="Header">
    <div class="logo-side">
    <img class="logo" src="../assets/imgs/logo.png" />
    <nav tag="h1" class="mb-1">DAY BETTER YOU</nav>
    </div>
    <div class="menu">
    <a class="home" href="">หน้าแรก</a>
    <a class="program" href="#">โปรแกรม</a>
    <a class="contact" href="#">ติดต่อเรา</a>
    <div class="button">
    <Button class="bt-begin"
    v-for="item in buttonText"
      :key="item.id"
      :text-title="item.textTitle"/>
    </div>
    </div>
</div>
</div>
</template>
<style lang="scss" >
@import '../styles/vars/color' ;
@import '../styles/vars/font' ;

    .Header{
    // position: absolute;
    color: #000000;
    background: #ffffff;
    height: 64px;
    width: 100%;
    // left: 0px;
    // top: 4px;
    border-radius: 0px;
    border-top: $main-color 4px solid;
    display: flex;
    justify-content: space-between;
    }
    .logo{
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    // position: absolute;
    height: 32px;
    width: 32px;
    border-radius: 0px;
    // top: 19px;
    margin-left:  56px;
    }
    .mb-1{
    // position: absolute;
    height: 26px;
    // left: 94px;
    // top: 23px;
    font-family: $main-font;
    font-size: 20px;
    font-style: normal;
    font-weight: 700;
    line-height: 26px;
    letter-spacing: 0px;
    text-align: left;
    color: $main-color;
    }
    .logo-side{
        display: flex;
        
    }
    .menu {
    position: relative;
    float:       right;
}
.menu a{
    list-style: none;
    display: inline-block;
    color: #000000;
    font-size: 14px;
    font-style: normal;
    font-weight: 400;
    line-height: 18px;
    padding: 30px;

}
.button{
    margin-left:  65px;
    margin-right: 56px;
    float:       right;
    position: relative;
    padding-top:  10px;
}

    </style>
    <script>
    import Button from '../components/Button'
     export default {
       data(){
           return{
            buttonText:[{
               id:2,
                textTitle:'เริ่มโปรแกรม'
              }
            ]
           }
     }
     }
    </script>