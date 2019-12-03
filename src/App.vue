<template>
  <div class="app">
    <div class="row">
      <Navheader class="header"></Navheader>
    </div>
    <router-view />
  </div>
</template>

<script>
import Navheader from "@/components/Header.vue";

export default {
  components: { Navheader }
};
</script>

<style>
*,
*::after,
*::before {
  box-sizing: border-box;
  margin: 0px;
  padding: 0px;
}
</style>
<style lang="scss" scoped>
.app {
  position: relative;
}
.row {
  position: sticky;
  left: 0px;
  top: 0px;
  z-index: 2;
}
</style>

