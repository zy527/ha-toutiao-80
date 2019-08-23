<template>
    <div class="container">
        <el-card class="box-card">
            <img src="../../assets/images/logo_index.png" style="margin-bottom: 40px">

            <el-form :model="loginForm" style="">
                <el-form-item>
                <el-input v-model="loginForm.mobile" placeholder="请输入你的手机号"></el-input>
                </el-form-item>

                <el-form-item>
                <el-input v-model="loginForm.code" placeholder="请输入你的验证码" style="width: 265px"></el-input>
                <el-button style="margin-left: 10px">验证码</el-button>
                </el-form-item>

                <el-button type="primary" round style="width: 100%">登录</el-button>
            </el-form>

        </el-card>

    </div>

</template>

<script>
export default {
  data () {
    return {
      loginForm: {
        mobile: '',
        code: ''
      }
    }
  }

}
</script>

<style lang="less" scoped>
.container {
    background: url(../../assets/images/login_bg.jpg) no-repeat center / cover;
    width: 100%;
    height: 100%;
    position: absolute;
    left: 0;
    top: 0
}

  .box-card {
    width: 400px;
    height: 350px;
    position: absolute;
    top: 20%;
    left: 30%;

    img {
        width: 200px;
        display: block;
        margin: 0 auto;
    }
  }

</style>
