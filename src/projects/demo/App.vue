<script>
export default {
  created () {
    /*
     * 平台 api 差异的处理方式:  api 方法统一挂载到 mpvue 名称空间, 平台判断通过 mpvuePlatform 特征字符串
     * 微信：mpvue === wx, mpvuePlatform === 'wx'
     * 头条：mpvue === tt, mpvuePlatform === 'tt'
     * 百度：mpvue === swan, mpvuePlatform === 'swan'
     * 支付宝(蚂蚁)：mpvue === my, mpvuePlatform === 'my'
     */
  }
}
</script>

<!--
  内置4种css解析器，默认使用postcss。
  lang="postcss"、lang="scss"
  lang="less"、lang="stylus"
-->
<style lang="postcss">
img {
  border: 0;
  vertical-align: top;
}
</style>
