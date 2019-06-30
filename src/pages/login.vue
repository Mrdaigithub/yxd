<template>
  <div class="login full-container">
    <div class="flex">
      <van-image
        class="login-img"
        :src="loginImg"/>
    </div>
    <v-text-field
      v-model="username"
      class="xx"
      label="请输入账号或手机号"
      prepend-icon="person"></v-text-field>
    <v-text-field
      v-model="password"
      label="请输入密码"
      prepend-icon="lock"></v-text-field>
    <div class="flex login-box">
      <van-button
        type="info"
        block
        round>登录
      </van-button>
    </div>
    <p class="text-center">新店铺注册</p>
    <div class="flex login-box">
      <van-button
        icon="wechat"
        type="default"
        block
        round>微信号登录
      </van-button>
    </div>
  </div>
</template>

<script>
import loginImg from '../assets/login.svg';

export default {
  name: 'Login',
  data() {
    return {
      loginImg: loginImg,
      username: 'root',
      password: 'root',
    };
  },
  methods: {},
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="stylus">
  .van-nav-bar
    background-color #ffffff

  .flex
    padding 46px 0 34px 0

  .login-img
    width 228px
    height 228px
    margin 0 24px

  .login-box
    margin: 32px 0 32px 0;

  .v-input
    font-size 28px!important

  .van-button
    height 94px
    line-height 94px

  .van-button--normal
    font-size 32px
    margin 0 24px
</style>
