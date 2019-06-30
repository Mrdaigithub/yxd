<template>
  <div class="hello content">
    <router-link to="/login">Go to login</router-link>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data() {
    return {
      msg: 'Welcome to Your Vue.js App',
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="stylus">
  .hello
    width 100vw
    height 100vh
    background-color #ffffff
</style>
