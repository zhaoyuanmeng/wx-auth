<!-- home -->
<template>
  <div class="app-container">
    <div class="warpper">
      <h1 class="demo-home__title"><img src="https://imgs.solui.cn/weapp/logo.png" /><span>VUE WECHAT AUTH</span></h1>
      <h2 class="demo-home__desc">
        vue 微信授权解决方案
      </h2>
    </div>
    <van-cell icon="success" v-for="item in list" :key="item" :title="item" />
    <van-tabbar fixed v-model="active" @change="onChange">
      <van-tabbar-item icon="home-o">首页</van-tabbar-item>
      <van-tabbar-item icon="good-job-o">github</van-tabbar-item>
    </van-tabbar>
  </div>
</template>

<script>
export default {
  components: {},

  data() {
    return {
      active: 0,
      list: ['vue 微信授权解决方案', '终于等到你', '还好没放弃']
    }
  },

  computed: {},

  mounted() {},

  methods: {
    onChange(index) {
      if (index === 1) window.location.href = 'https://github.com/sunnie1992/vue-wechat-auth'
    }
  }
}
</script>
<style scoped></style>
