<template>
    <div class="tab-data">
        <div class="banner-block">
          <div class="banner-left">
                <div class="banner-text">
                  โดยผู้เชี่ยวชาญ
                </div>
                <div class="banner-sub-text">
                  เนื้อหาจำลองแบบเรียบๆ ที่ใช้กันในธุรกิจงานพิมพ์
                </div>
                </div>
              <div class="banner-icon">
                <img src="../assets/imgs/icon.png">
              </div>
              </div>
              <div class="banner-block">
                <div class="banner-left">
                <div class="banner-text">
                  ได้ผลจริง
                </div>
                <div class="banner-sub-text">
                  เนื้อหาจำลองแบบเรียบๆ ที่ใช้กันในธุรกิจงานพิมพ์
                </div>
                </div>
              <div class="banner-icon">
                <img src="../assets/imgs/icon1.png">
              </div>
              </div>
              <div class="banner-block">
                <div class="banner-left">
                <div class="banner-text">
                  ทุกที่ทุกเวลา
                </div>
                <div class="banner-sub-text">
                  เนื้อหาจำลองแบบเรียบๆ ที่ใช้กันในธุรกิจงานพิมพ์
                </div>
                </div>
              <div class="banner-icon">
                <img src="../assets/imgs/icon2.png"/>
      </div>
              </div>
    </div>
</template>
<style lang="scss" scoped>
.tab-data{
      font-family: $main-font;

  position: absolute;
  align-content: center;
  height: 127px;
width: 960px;
bottom: 0;
background: rgba(255, 255, 255, 0.3);
display: flex;
  justify-content: center;
border-radius: 6px 6px 0px 0px;
margin-left: 13%;
}
.banner-block{
  width: 320px;
  display: flex;
  justify-content: space-between;
  padding: 32px ;
}
.banner-block:first-child{
  border-right: 1px solid rgba(255, 255, 255, 0.25);
}
.banner-block:last-child{
  border-left: 1px solid rgba(255, 255, 255, 0.25) ;
}
.banner-text{
  
      color:#FFFFFF;
      font-style: normal;
      font-weight: 700;
      line-height: 21px;
      height: 21px;
}
.banner-sub-text{
    color:#FFFFFF;
font-size: 12px;
font-style: normal;
font-weight: 400;
line-height: 16px;
height: 32px;
width: 164px;
}
.banner-icon{
    height: 50px;
width: 50px;
top: 525px;
float: right;

}
</style>