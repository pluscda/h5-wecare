<template>
  <div>
    <h3 class="navheader"><img :src="img" width="100%" ></img></h3>
  </div>
</template>

<script>
export default{
  data(){
    return {
      img: require('@/assets/images/components/1-01.png')
    }
  }
}

</script>

<style>
.navheader{
  background-color: #2699FB;
  height: 100%;
  padding: 10px;
  box-shadow: 0px 9px 12px rgba(0,0,0,0.3);

}
</style>
