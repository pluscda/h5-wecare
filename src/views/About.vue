<template>
  <div class="about">
    
    <div class="content">
      <van-row class="button">
        <van-col span="24"><van-button color="linear-gradient(to top, #0071BC, #4bb0ff)" size="large" type="info">我的累積評價</van-button></van-col>
      </van-row>
      <van-row class="button">
        <van-col span="24"><van-button color="linear-gradient(to top, #0071BC, #4bb0ff)" size="large" type="info">查看選手紀綠</van-button></van-col>
      </van-row >
      <van-row class="button">
        <van-col span="24"><van-button to="/personal" color="linear-gradient(to top, #0071BC, #4bb0ff)" size="large" type="info">我的個人設定</van-button></van-col>
      </van-row>
      <van-row class="button">
        <van-col span="24"><van-button color="linear-gradient(to top, #0071BC, #4bb0ff)" size="large" type="info">收入帳戶</van-button></van-col>
      </van-row>
      <van-row class="button">
        <van-col span="24"><van-button color="linear-gradient(to top, #0071BC, #4bb0ff)" size="large" type="info">收入歷史清單</van-button></van-col>
      </van-row>
      <van-row class="button">
        <van-col span="24"><van-button to="/" color="linear-gradient(to top, #0071BC, #4bb0ff)" size="large" type="info">登出帳號</van-button></van-col>
      </van-row>    
    </div>
    <myschedulebutton>
    </myschedulebutton>
    
    
  </div>
</template>
<script>
import myschedulebutton from  '@/components/Myschedulebutton'
export default {
  components: {myschedulebutton},
}
</script>
<style>
html, body{
  height:100%;
  width:100%;
}
*{
  text-align: center;
  position: relative;
}
.about{
  height: 100%;
}
.content{
  box-shadow: 0px 9px 12px rgba(0,0,0,0.3);
  height: 80% ;
  padding-bottom: 20px;
}
.button{
  width:80%;
  margin: 5% 0px;
  margin-left: auto;
  margin-right: auto;

  padding: 0px;
  border-radius: 10px;
  overflow:hidden;
}
.block{
  display: flex;
  justify-content: center;
  align-items: center;
  height: 20%;
  width:100%;

}
.Box{
  padding: 10px 0px;
}
</style>
