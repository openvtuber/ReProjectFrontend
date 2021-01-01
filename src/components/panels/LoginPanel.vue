<template>
  <!-- Designed by Archeb https://qwq.moe/ -->
  <!-- 使用此 UI 必须经过 Archeb & FENGberd 授权 -->
  <!-- Modify & move to Vue by Gerard -->
  <div class="login">
    <div class="single-bg"></div>
    <div class="notify-container"></div>
    <div class="main padding-limiter">
      <div class="panel login-panel">
        <div class="double-column">
          <img class="panel-wide login-img" src="/image/login.jpg" />
          <div class="panel-narrow" id="p-login">
            <div class="title">
              Nyatwork 登录
            </div>
            <div class="control-group">
              <label>账户</label>
              <div class="controls">
                <input
                  id="username"
                  type="text"
                  placeholder="用户名/邮箱/手机号"
                  title="账户"
                />
              </div>
            </div>
            <div class="control-group">
              <label>密码</label>
              <div class="controls">
                <input id="password" type="password" title="密码" />
              </div>
            </div>
            <div style="text-align: right">
              <label>
                <a href="/register">注册</a>
                <a
                  href="/reset_password"
                  style="margin: 0 60px 0 8px"
                  class="wtf-fix"
                  >忘记密码?</a
                >
              </label>
            </div>
            <div class="actions">
              <button class="btn" id="login">登录</button>
            </div>
          </div>
          <div class="panel-narrow" id="p-2fa" style="display: none;">
            <div class="title">
              两步验证
            </div>
            <div class="control-group">
              <label>代码</label>
              <div class="controls">
                <input id="2fa" type="text" title="两步验证代码" />
              </div>
            </div>
            <div class="actions">
              <button class="btn" id="login_2fa">提交</button>
            </div>
          </div>
          <div class="panel-narrow" id="p-u2f" style="display: none;">
            <div class="title">
              :)
            </div>
            <div
              id="u2f_status"
              style="text-align: center;margin-right: 15px;"
            ></div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "LoginPanel"
};
</script>

<style lang="less" scoped>
@import url("/css/base.min.css");
@import url("/css/notify.min.css");
</style>
