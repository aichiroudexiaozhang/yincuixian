<template>
  <div>
    <van-nav-bar title="标题" />
    <form>
      <van-cell-group>
        <van-field v-model="form.name"
                   required
                   clearable
                   label="用户名"
                   placeholder="请输入用户名" />

        <van-field v-model="form.code"
                   type="password"
                   label="密码"
                   placeholder="请输入密码"
                   required />
      </van-cell-group>
      <div class="lang_btn">
        <van-button class="btn"
                    type="info">登录</van-button>
      </div>
    </form>
  </div>
</template>

<script>
export default {
  name: 'AppLogIN',
  data () {
    return {
      form: {
        name: '',
        code: ''
      }
    }
  }

}
</script>

<style lang="less" scoped>
.lang_btn {
  padding-top: 20px;
  .btn {
    width: 100%;
  }
}
</style>
