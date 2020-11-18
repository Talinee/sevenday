<template>
      <div class="block">
            <figure>
            <img class="bg" src="../assets/img/bg.jpg">
      </figure>
      <h1 class="title">7 DAYS BETTER YOU</h1>
      <h2 class="subtitle">เนื้อหาจำลองแบบเรียบๆ ที่ใช้กันในธุรกิจงานพิมพ์หรืองานเรียงพิมพ์<br>
       มันได้กลายมาเป็นเนื้อหาจำลองมาตรฐานของธุรกิจดังกล่าวมาตั้งแต่ศตวรรษที่ 16 </h2>
      <Button class="bt-regis">สมัครสมาชิก</Button>
      <div class="tab-data">
                <div class="banner-tab">
                  โดยผู้เชี่ยวชาญ
                </div>
                <div class="banner-sub-tab">
                  เนื้อหาจำลองแบบเรียบๆ ที่ใช้กันในธุรกิจงานพิมพ์
                </div>
              <div class="banner-icon">
                <img src="../assets/img/icon.png">
              </div>
            <div class="banner-tab">
                <div class="banner-tab">
                  ได้ผลจริง
                </div>
                <div class="banner-sub-tab">
                  เนื้อหาจำลองแบบเรียบๆ ที่ใช้กันในธุรกิจงานพิมพ์
                </div>
              </div>
              <div class="banner-icon">
                <img src="../assets/img/icon1.png">
              </div>
                <div class="banner-tab">
                  ทุกที่ทุกเวลา
                </div>
                <div class="banner-sub-tab">
                  เนื้อหาจำลองแบบเรียบๆ ที่ใช้กันในธุรกิจงานพิมพ์
                </div>
              </div>
              <div class="banner-icon">
                <img src="../assets/img/icon2.png">
      </div>
      <div class="section-1">
            <div class="sec1-title">
               <title>เปลี่ยนเป็นคุณคนใหม่ใน 7 วัน</title>
            </div>
            <div class="sec1-subtitle">
                  <title>เนื้อหาจำลองแบบเรียบๆ ที่ใช้กันในธุรกิจงานพิมพ์หรืองานเรียงพิมพ์ 
                        <br>
                        มันได้กลายมาเป็นเนื้อหาจำลองมาตรฐานของธุรกิจดังกล่าวมาตั้งแต่ศตวรรษที่ 16
                  </title>
            </div>
            <img class="sec1-img" src="../assets/img/image 3.png">
      </div>
      <div class="section-2">
            <div class="pop-program">
                  โปรแกรมยอดนิยม
                  <Card
                     v-for="item in popList"
                     :key="item.id"
                     :src="item.img"
                     :main-message="item.mainMessage"
                     :sub-message="item.subMessage"
                     :price="item.price"/>
            </div>
      </div>
       <div class="section-3">
            <img class="banner" src="../assets/img/stats.jpg"/>
      </div>
      </div>
</template>
<script>
import Card from '../components/Card'

export default {
  components: {
    Card
  },
  data () {
    return 
      popList: [
        {
          id: 1,
          img: require('../assets//img/Group 4.png'),
          mainMessage: 'สร้างความมั่นใจ',
          subMessage: 'เติมพลังความมั่นใจ ให้ทุกวันเป็นวันทีทรงพลัง',
          price: 'ฟรี'
        },
        {
          id: 2,
          img: require('../assets/img/Group42.png'),
          mainMessage: 'สร้างความมั่นใจ',
          subMessage: 'เติมพลังความมั่นใจ ให้ทุกวันเป็นวันทีทรงพลัง',
          price: '0฿'
        },
        {
          id: 3,
          img: require('../assets/img/Group 43.png'),
          mainMessage: 'สร้างความมั่นใจ',
          subMessage: 'เติมพลังความมั่นใจ ให้ทุกวันเป็นวันทีทรงพลัง',
          price: '0฿'
        },
        {
          id: 4,
          img: require('../assets/img/Group 44.png'),
          mainMessage: 'สร้างความมั่นใจ',
          subMessage: 'เติมพลังความมั่นใจ ให้ทุกวันเป็นวันทีทรงพลัง',
          price: '0฿'
        }
      ]
  }
  }
</script>

<style lang="scss">
  .bg{
    position: absolute;
    height: 560px;
    width: 100%;
    top: 68px;
    object-fit: cover;
    
    }
    .title{
    position: absolute;
            top:174px;
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
          position: absolute;
            width: 100%;
            display: flex;
                text-align: center;
                Top :260px;
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
    position: absolute;
    height: 48px;
    width: 152px;
    left: 50%;
    margin-right: -50%;
    transform: translate(-50%, -50%) ;
    top: 354px;
    }
    .tab-data{
          position: absolute;
          align-content: center;
    height: 127px;
width: 74%;
top: 501px;
background: rgba(255, 255, 255, 0.3);
display: flex;
  justify-content: center;
border-radius: 6px 6px 0px 0px;
margin-left: 13%;
}
.banner-tab{
      display: flex;
      flex-direction: column;
      color:#FFFFFF;
      font-size: 16px;
      font-weight: 700;
      margin-bottom: 5px;
}
    .section-1{
    position: absolute;
    height: 480px;
    width: 100%;
    top: 628px;
    background: #FFFFFF;
    }
    .sec1-title {
    position: absolute;
    height: 42px;
    width: 100%;
    top: 70px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    }
    .sec1-title title{
          position: absolute;
    font-family: $main-font;
    font-style: normal;
    font-size: 32px;
    font-weight: 700;
    line-height: 42px;
    letter-spacing: 0px;
    text-align: center;
    color: #000000;
    display: flex;
    flex-direction: column;
    }
    .sec1-subtitle title{
          position: absolute;
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
          position: absolute;
    height: 315px;
    width: 581px;
    left: 433px;
    top: 213px;
    border-radius: 0px;
    }
    .section-2{
           position: absolute;
          height: 740px;
width: 100%;
left: 0px;
top: 1108px;
background: #F6F8FA;
    }
    .banner {
width: 100%;
height: 300px;
position: absolute;
top: 1848px;

    }


</style>
