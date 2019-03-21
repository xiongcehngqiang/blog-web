<template>
  <div class="hover">
    <div class="contain">{{contant}}</div>
    <div class="bottom"></div>
  </div>
</template>

<script>
export default {
  name: "hover",
  props: ["contant"]
}
</script>

<style lang='scss'>
.hover {
  min-width: 0px;
  height: 100%;
  position: relative;
  overflow: hidden;
  .contain {
    justify-content: center;
    height: 100%;
    display: flex;
    align-items: center;
  }
  .bottom {
    position: absolute;
    width: 100%;
    height: 4px;
    background: #09f;
    bottom: -4px;
    transition: all 0.3s;
  }
}
.hover:hover {
  color: #09f;
}
.hover:hover .bottom {
  bottom: 0px;
}
</style>
