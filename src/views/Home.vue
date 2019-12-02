<template>
  <div class="login">
    <van-row class="logo">
      <van-col span="24"><van-image :src="img"/></van-col>
    </van-row>

    <van-row class="button">
      <van-col span="24"><van-button to="/registered" size="large" type="info">註冊</van-button></van-col>
    </van-row>
    <van-row class="button">
      <van-col span="24"><van-button to="/about" size="large" type="info">登入</van-button></van-col>
    </van-row>
  </div>
</template>

<script>
export default{
  data(){
    return{
      img: require("@/assets/images/login/WeCare_logo.png")
    }
  }
}
</script>

<style>
html, body {
  width:100%;
  height:100%;
}
.login {
  background-image:url('../../src/assets/images/login/bgimg.png');
  background-size: cover;
  height: 700px;
  box-sizing: border-box;
  position: absolute ;
  width: 100%;
  /* 這裡背景圖希望不要讓它滾動 */
}
* {
  position: relative;
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  margin: 0px;
  text-align: center;
}
.logo {
  margin-top: 100px;
  margin-bottom: 30px;
  width: 50%;
  margin-left: auto;
  margin-right: auto;
}
.button{
  padding: 0px;
  margin: 5px;
  width: 30%;
  margin-left: auto;
  margin-right: auto;
  border-radius: 10px;
  overflow:hidden;
  box-shadow: 0px 9px 12px rgba(0,0,0,0.2);

}

</style>
