<template>
  <div class="personal">
    <BasicInfor></BasicInfor>
    <van-cell-group title="聯絡方式">
      <van-field label="聯絡電話" />
      <van-field label="聯絡手機" />
      <van-field label="E-mail" />
      <van-field label="縣市" />
      <van-field label="行政區" />
      <van-field label="地址" />
    </van-cell-group>
    <van-row class="button">
      <van-col span="24"><van-button to="/about" color="linear-gradient(to top, #4bb0ff, #0071BC)" size="large" type="info">確定</van-button></van-col>
    </van-row>
  </div>
  
</template>

<script>
import BasicInfor from '@/components/BasicInformation'
export default {
  components: { BasicInfor },
  data() {
    return {
      
    }
  },

  methods: {
  }
};
</script>

<style>
.personal{
  background-color: #F8F8F8;
}
BasicInfor{
  color: red;
}

</style>
