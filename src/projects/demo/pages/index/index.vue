<template>
  <div class="index-page">
    <div class="content">
      <img src="./imgs/user.png" alt="">
      <div class="text">--- 基于mpVue小程序工程化实践 ---</div>
    </div>
  </div>
</template>

<script>

export default {
  data () {
    return {
    }
  },

  components: {
  },

  methods: {
  }
}
</script>

<style lang="postcss" scoped>
.index-page {
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
}
.content {
  text-align: center;
  padding-bottom: 150px;
  img {
    width: 200px;
    height: 200px;
  }
}
.text {
  font-size: 14px;
}
</style>
