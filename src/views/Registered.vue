<template>
  <div class="personal">
    <BasicInfor></BasicInfor>
    <div class="InputBlock">
      <van-row type="flex" justify="center">
        <van-col class="colstyle" span="20">
          <van-field
            label="會員帳號:"
            placeholder="請輸入帳碼"
          />
        </van-col>
      </van-row>
      <van-row type="flex" justify="center">
        <van-col class="colstyle" span="20">
          <van-field
            label="會員密碼:"
            placeholder="請輸入密碼"
          />
        </van-col>
      </van-row>
      <van-row type="flex" justify="center">
        <van-col class="colstyle" span="20">
          <van-field
            label="確認密碼:"
            placeholder="請重新輸入密碼"
          />
        </van-col>
      </van-row>
      

    </div>
    <van-row class="button">
      <van-col span="24"><van-button to="/personal" color="linear-gradient(to top, #0071BC, #4bb0ff)" size="large" type="info">確定</van-button></van-col>

      </van-popup>
    </van-row>
  </div>
  
</template>

<script>
import BasicInfor from '@/components/BasicInformation'
export default {
  components: { BasicInfor },
  data() {
    return{

    }
  },

  methods: {
    
  }
};
</script>

<style>
.InputBlock{
  background-color: #2699FB;
  height: 100%;
  padding: 20px;
}
.colstyle{
  margin: 5px;
}
.personal{
  background-color: #F8F8F8;
}


</style>
