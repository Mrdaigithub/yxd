<template>
  <div class="foo">
    <van-button type="info" @click="gotoHome">asasd</van-button>
    <h1>foo</h1>
  </div>
</template>

<script>
export default {
  name: 'foo',
  data() {
    return {
      msg: 'Welcome to Your Vue.js App',
    };
  },
  methods: {
    gotoHome() {
      this.$router.go(-1);
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="stylus">
  .foo
    width 100vw
    height 100vh
    background-color #fff

  h1
    font-size 200px
</style>
