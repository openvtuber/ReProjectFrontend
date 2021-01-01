<template>
  <div>
    <Background class="bg" />
    <LoginPanel class="login_panel" />
  </div>
</template>
<script>
import Background from "@/components/utils/Background.vue";
import LoginPanel from "@/components/panels/LoginPanel.vue";
export default {
  components: { Background, LoginPanel }
};
</script>
<style lang="less" scoped>
.bg {
  position: absolute;
  z-index: -999;
}
.login_panel {
  position: relative;
  z-index: 1;
  left: 50%;
  transform: translate(-50%, 50%);
}
</style>
