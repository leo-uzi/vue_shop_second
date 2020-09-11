<template>
  <div class="container">
    <el-button type="info" @click="handleLogout">退出</el-button>
  </div>
</template>

<script>
export default {
  data () {
    return {

    }
  },
  methods: {
    handleLogout () {
      window.sessionStorage.clear()
      this.$router.push('/login')
    }
  }
}
</script>

<style scoped lang="less">

</style>
