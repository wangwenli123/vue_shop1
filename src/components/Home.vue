<template>
  <div>
    <elbutton type="info" @click="logout">退出</elbutton>
  </div>
</template>
<script>
export default {
  methods: {
    logout() {
      window.sessionStorage.clear()
      this.$router.push('/login')
    }
  }
}
</script>
<style lang="less" scoped></style>
