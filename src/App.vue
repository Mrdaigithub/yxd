<template>
  <div id="app" class="full-container">
    <van-nav-bar
      title="asdasd"
      left-arrow
      @click-left="backUrl"/>
    <router-view v-transition/>
  </div>
</template>

<script>
export default {
  name: 'App',
  methods: {
    backUrl() {
      this.$router.go(-1);
    },
  },
};
</script>

<style>
</style>
