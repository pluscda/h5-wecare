<template>
  <div>
    <Navheader></Navheader>
    <router-view/>
  </div>
</template>

<script>
import Navheader from '@/components/header.vue'

export default {
	components: { Navheader },
}
</script>

<style>
/*.NavBar{
  height: 20%;
  background-color: red;
}*/
</style>
