<template>
  <div class="personal">
    <van-cell-group title="個人基本資料">
      <van-field
        clearable
        label="姓:"
        required
        input-align="center"

      />
      <van-field
      clearable
      label="名:"
      required
      input-align="center"
      />
      <van-field
      clearable
      label="身分證:"
      required
      placeholder="請輸入用户名"
      input-align="center"
      />


      <van-field
        is-link
        readonly
        required
        clickable
        label="性別:"
        :value="value_sex"
        placeholder="選擇性別"
        @click="showPickerSex = true"
      />

      <van-popup v-model="showPickerSex" position="bottom" :style="{ height: '50%' }"> 
        <van-picker
          show-toolbar
          :columns="sexs"
          confirm-button-text="確認"
          @cancel="showPickerSex = false"
          @confirm="onConfirmSex"
        />
      </van-popup>
      <van-field
        is-link
        readonly
        required
        clickable
        label="生日:"
        :value="birthvalue"
        placeholder="填寫日期"
        @click="showPickerBirthday = true"
      />

      <van-popup v-model="showPickerBirthday" position="bottom" :style="{ height: '50%' }"> 
        <van-datetime-picker
          confirm-button-text="確認"
          @confirm="onConfirmBirth"
          
          v-model="currentDate"
          type="date"
          :min-date="minDate"
        />
      </van-popup>
      <van-field
        is-link
        readonly
        required
        clickable
        label="年齡:"
        :value="value_age"
        placeholder="填寫年齡"
        @click="showPickerAge = true"
      />

      <van-popup v-model="showPickerAge" position="bottom" :style="{ height: '50%' }"> 
        <van-picker
          show-toolbar
          :columns="ages"
          confirm-button-text="確認"
          @cancel="showPickerSex = false"
          @confirm="onConfirmAge"
        />
      </van-popup>

    </van-cell-group>

      <van-cell-group title="看護訊息">
        <van-cell title="看護證照" value="尚未更新資料" is-link to="/carelicense" title-class="title"/>
        <van-cell title="可服務區域" value="尚未更新資料" is-link to="/" title-class="title"/>
        <van-cell title="可服務時段" value="尚未更新資料" is-link to="/" title-class="title"/>
        <van-cell title="服務經歷" value="尚未更新資料" is-link to="/carelicnse" title-class="title"/>
      
    </van-cell-group>
  </div>
  
</template>

<script>
export default {
  data() {
    return {
      show: false,
      value: '',
      value1: '123e',


      value_sex: '',
      showPickerSex: false,
      sexs: ["F","M","O"],

      birthvalue: null,
      //資料的型態要在查一下
      showPickerBirthday: false,
      currentDate: new Date(),
      minDate: new Date(),

      value_age: '',
      showPickerAge: false,
      ages: [18,19,20,21,22,23,24],
    }
  },

  methods: {
    showPopup() {
      this.show = true;
    },
    onConfirmSex(value) {
      this.value_sex = value;
      this.showPickerSex = false;
    },
    onConfirmAge(value) {
      this.value_age = value;
      this.showPickerAge = false;
    },
    onConfirmBirth(value) {
      this.birthvalue = value;
      this.showPickerBirthday = false;
    }
  }
};
</script>

<style>
.personal{
  background-color: #F8F8F8;
}
.title{
  text-align: left;
  padding-left: 10px;
}
</style>
