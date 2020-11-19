<template>
      <div class="block">
            <div class="block-1">
                <!-- <img class="bg" src="../assets/imgs/bg.jpg"> -->
                <h1 class="title">7 DAYS BETTER YOU</h1>
                <h2 class="subtitle">เนื้อหาจำลองแบบเรียบๆ ที่ใช้กันในธุรกิจงานพิมพ์หรืองานเรียงพิมพ์<br>
                มันได้กลายมาเป็นเนื้อหาจำลองมาตรฐานของธุรกิจดังกล่าวมาตั้งแต่ศตวรรษที่ 16 </h2>
                <Button class="bt-regis"
                text-title="สมัครสมาชิก"
                /> 
                <Datatab/>
            </div>
      <div class="section-1">
            <div class="sec1-title">
               <p>เปลี่ยนเป็นคุณคนใหม่ใน 7 วัน</p>
            </div>
            <div class="sec1-subtitle">
                  <p>เนื้อหาจำลองแบบเรียบๆ ที่ใช้กันในธุรกิจงานพิมพ์หรืองานเรียงพิมพ์ 
                        <br>
                        มันได้กลายมาเป็นเนื้อหาจำลองมาตรฐานของธุรกิจดังกล่าวมาตั้งแต่ศตวรรษที่ 16
                  </p>
            </div>
            <img class="sec1-img" src="../assets/imgs/image 3.png">
      </div>
      <div class="section-2">
            <div class="pop-program">
                  โปรแกรมยอดนิยม
                  </div>
                  <div class="card">
                      <Card class="pop-card"
                        v-for="item in popList"
                        :key="item.id"
                        :src="item.img"
                        :main-message="item.mainMessage"
                        :sub-message="item.subMessage"
                        :price="item.price"/>
                     </div>
                     <Button class="see-all"
        textTitle="ดูทั้งหมด"/>
      </div>
       <div class="section-3">
            <img class="banner" src="../assets/imgs/stats.jpg"/>
      </div>
      <div class="section-4">
        <div class="mobile-content">
        <img class="download-app" src="../assets/imgs/Black iPhone.png">
        <img class="download-icon" src="../assets/imgs/app.png">
        </div>
      </div>
      <div class="section5">
        <div class="sec5-bg">
         <img class="pic-peopel" src="../assets/imgs/Group 16.png">
         </div>
      </div>
      </div>
</template>
<script>
import Card from '../components/Card'
import Button from '../components/Button'

export default {
  components: {
    Card,Button
  },
  data () {
    return {
      popList: [
        {
          id: 1,
          img: require('../assets/imgs/Group 4.png'),
          mainMessage: 'สร้างความมั่นใจ',
          subMessage: 'เติมพลังความมั่นใจ ให้ทุกวันเป็นวันทีทรงพลัง',
          price: 'ฟรี'
        },
        {
          id: 2,
          img: require('../assets/imgs/Group42.png'),
          mainMessage: 'สร้างความมั่นใจ',
          subMessage: 'เติมพลังความมั่นใจ ให้ทุกวันเป็นวันทีทรงพลัง',
          price: '0฿'
        },
        {
          id: 3,
          img: require('../assets/imgs/Group 43.png'),
          mainMessage: 'สร้างความมั่นใจ',
          subMessage: 'เติมพลังความมั่นใจ ให้ทุกวันเป็นวันทีทรงพลัง',
          price: '0฿'
        },
        {
          id: 4,
          img: require('../assets/imgs/Group 44.png'),
          mainMessage: 'สร้างความมั่นใจ',
          subMessage: 'เติมพลังความมั่นใจ ให้ทุกวันเป็นวันทีทรงพลัง',
          price: '0฿'
        }
      ],
    }
  }
  }
</script>

<style lang="scss">
.block-1{
  background-image: url(../assets/imgs/bg.jpg);
  background-size: cover;
  height: 560px;
  background-repeat: no-repeat;
  display: flex;
  flex-direction: column;
  justify-content: center;
  position: relative;


}
    .title{
            color:#fff;
            width: 100%;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            font-weight: 500;
            font-size:40px;
            text-align: center;
    
    }
    .subtitle{
            width: 100%;
            display: flex;
                text-align: center;
                font-weight: 400;
                font-family: $main-font;
            flex-direction: column;
            justify-content: center;
            font-style: normal;
            align-items: center;
            font-size:14px;
            line-height:20px;

    
    text-align: center;
    
    color: #FFFFFF;
    
    mix-blend-mode: normal;
    opacity: 0.85;
    }
    .bt-regis{
    height: 48px;
    width: 152px;
    margin: 0 auto;
    }
    .section-1{
    // position: absolute;
    height: 480px;
    width: 100%;
    // top: 628px;
    background: #FFFFFF;
    }
    .sec1-title {
    height: 42px;
    width: 100%;
    text-align: center;
    }
    .sec1-title p{
    font-family: $main-font;
    font-style: normal;
    font-size: 32px;
    font-weight: 700;
    line-height: 42px;
    letter-spacing: 0px;
    text-align: center;
    color: #000000;
    }
    .sec1-subtitle p{
    height: 48px;
    width: 100%;
    top: 133px;
    font-family: $main-font;
    font-style: normal;
    font-weight: normal;
      font-size: 14px;
      line-height: 24px;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
    /* or 171% */
    
    text-align: center;
    
    color: #000000;
    
    mix-blend-mode: normal;
    opacity: 0.65;
    }
    .sec1-img{
    height: 315px;
    width: 581px;
    margin: 0 auto;
    display: block;
    }
    .section-2{
           position: absolute;
          height: 740px;
width: 100%;
left: 0px;
top: 1108px;
background: #F6F8FA;
    }
    .pop-program{
      margin: 72px 0px 0px 146px;
    }
    .card{
      display: grid;
      grid-template-columns: 280px 280px 280px 280px;
      grid-gap: 16px;
      justify-content: center;
      margin: 16px 21px 21px 21px;
    }
    .banner {
width: 100%;
height: 300px;
position: absolute;
top: 1848px;

    }
.popProgram{
        width: 100%;
        height: 740px;
        padding-top: 80px;
}
.see-all{
   height: 48px;
    width: 152px;
    margin: 0 auto;
    display: block;
}
.section-4{
}
.mobile-content{
  position: relative;
  
}
.download-app{
  height: 795px;
  width: 390px;
  top: 1116px;
  position: absolute;
  margin: 0px 0px 188px 188px;
}
.download-icon{
  height: 127px;
width: 127px;
position:absolute;
top: 1120px;
}
.section-5{
  height: 472px;
width: 100%;
top: 2770px;
}
.sec5-bd{
}
.pic-people{
    height: 256px;
    width: 608px;
    top: 2878px;
    border-radius: 2px;
    position: absolute;
    }
</style>
