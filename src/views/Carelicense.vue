<template>
  <div>
    <h4>看護證照請上傳</h4>
    <div class="licensebox">
      <div class="box">
        <img :src="img[0]" width="100%" >
        <h2>看護證照(正面)</h2>

      </div>
      <div class="Img">
        <img :src="img[1]" />
        <img :src="img[2]" />
      </div>
    </div>
    <div class="licensebox">
      <div class="box">
        <img :src="img[0]" width="100%" >
        <h2>看護證照(背面)</h2>

      </div>
      <div class="Img">
        <img :src="img[1]" />
        <img :src="img[2]" />
      </div>
    </div>


  </div>
</template>

<script>
export default{
  data(){
    return {
      img: [
        require("@/assets/images/carelicense/photo.png"),
        require("@/assets/images/carelicense/photoupdate.png"),
        require("@/assets/images/carelicense/cameraupdate.png"),
      ]
    }
  }
}
</script>

<style>
*{
  /* border: 1px solid; */
}
.licensebox{
  width: ;
}
h4{
  text-align: left;
  padding: 15px;
  margin-top: 5px;
}
.box img{
  width: 30%;
  border-radius: 50%;
  background-color: white;
}
.Img{
  /* position: relative;
  float: right; */
  /* float: right; */
}
.box{
  width:80%;
  background-color: #F8F8F8;
  margin: 20px 0px;
  margin-left: auto;
  margin-right: auto;
  padding: 30px 0px;
  border-radius: 5%;

}

</style>
