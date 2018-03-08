<template>
  <div class="site-content site-content--home">
    <el-card :style="contentViewStyles">
      <h3>欢迎使用Thplus后台管理系统</h3>
    </el-card>
  </div>
</template>

<script>
  export default {
    data () {
      return {
      }
    },
    computed: {
      contentViewStyles () {
        var height = this.$store.state.documentClientHeight
        height -= 50 // site-topbar
        height -= 15 // site-content padding-top
        height -= 15 // site-content padding-bottom
        height += 'px'
        return [
          { minHeight: height }
        ]
      }
    }
  }
</script>

<style>
  .site-content--home {
    line-height: 1.5;
  }
</style>

