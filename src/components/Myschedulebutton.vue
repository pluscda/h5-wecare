<template>
  <div class="block">
    <div class="Box">
      <van-row gutter="20">
        <van-col span="8"><van-image width="100" height="100" :src="img[0]"/></van-col>
        <van-col span="8"><van-image width="100" height="100" :src="img[1]"/></van-col>
        <van-col span="8"><van-image width="100" height="100" :src="img[2]"/></van-col>
      </van-row>      
    </div> 
  </div>
</template>

<script>
export default{
  data(){
    return {
      img:[
        require('@/assets/images/components/myschedule.png'),
        require('@/assets/images/components/booking.png'),
        require('@/assets/images/components/todaycaring.png'),
      ] 
    }
  }
}

</script>

<style scoped lang="scss">
.block{

  display: flex;
  justify-content: center;
  align-items: center;
  height: 20%;
  width:100%;
  margin-top:10px

}
.Box{
  padding: 10px 0px;
}
</style>
