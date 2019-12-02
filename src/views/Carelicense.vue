<template>
  <div>
    <h4>看護證照請上傳</h4>
    <div class="box">
      <img :src="img" width="100%" >
      <h2>看護證照</h2>
    </div>
    <div class="box">
      <img :src="img" width="100%" >
      <h2>看護證照</h2>
    </div>


  </div>
</template>

<script>
export default{
  data(){
    return {
      img: require("@/assets/images/carelicense/photo.png")
    }
  }
}
</script>

<style>
h4{
  text-align: left;
  padding: 15px;
  margin-top: 5px;
}
.box img{
  width: 30%;
  border-radius: 50%;
}
.box{
  width:80%;
  background-color: #F8F8F8;
  margin: 20px 0px;
  margin-left: auto;
  margin-right: auto;
  padding: 30px 0px;
}

</style>
