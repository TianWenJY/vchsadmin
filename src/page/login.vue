<template>
  <div class="main">
    <section>
      <img src="../images/login/logo.png" alt="">
    <form>
      <div class="form-group">
        <!--<label for="exampleInputEmail1">-->

        <input type="text" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp" placeholder="请输入用户名">
        <i class="people"></i>
        <!--</label>-->
        <!--<small id="emailHelp" class="form-text text-muted">We'll never share your email with anyone else.</small>-->
      </div>
      <div class="form-group">
        <!--<label for="exampleInputPassword1">-->
          <i class="pass"></i>
        <input type="password" class="form-control" id="exampleInputPassword1" placeholder="请输入密码">
        <!--</label>-->
      </div>
      <!--<div class="form-check">-->
        <!--<input type="checkbox" class="form-check-input" id="exampleCheck1">-->
        <!--<label class="form-check-label" for="exampleCheck1">Check me out</label>-->
      <!--</div>-->
      <div class="form-group mbtn">
      <button type="submit" class="btn btn-primary btn-block">登录</button>
      </div>
    </form>
    </section>
  </div>



</template>

<script type="text/ecmascript-6">
  // export default {
  //   name: 'Login',
  //   data() {
  //     return {
  //       loginForm: {
  //         username: '',
  //         password: '',
  //       },
  //       showLogin: false,
  //     }
  //   },
  //   methods: {
  //     submitForm:function() {
  //       this.$http.post(
  //         'http://api.cheshili.com.cn:8000/Admin/Login/LG',
  //         {
  //
  //           AdminName: this.loginForm.username,
  //           Password: this.loginForm.password,
  //           Platform: '23',
  //           Mobile: 1,
  //         },
  //         // {
  //         //   headers: {'Content-Type': 'application/x-www-form-urlencoded'}
  //         // }
  //         {emulateJSON: true}
  //       ).then((res) => {
  //         res = res.body;
  //         if(res.Status == 0 && res.Data) {
  //           // $$.setToken(res.Data.WToken);
  //           sessionStorage.setItem('__UINFO__',res.Data.Info);
  //           this.$router.push({ path: '/index'})
  //         }
  //       }),function (err){
  //         console.log(err)
  //       }
  //     }
  //   }
  // }


</script>

<style>
  .main {
    position: relative;
    overflow: hidden;
    width: 100%;
    height: 100%;
    background:url(../images/login/bg.jpg) no-repeat;
    background-size: cover;
  }
  div.main > section {
    width: 100%;
    background-color: rgba(0, 0, 0, 0.4);
    position: absolute;
    text-align: center;
    top: 30%;
    height: 240px;
    transition: height 0.4s, top 0.4s;
  }
  html {
    overflow: hidden;
    height: 100%;
  }
  @media screen and ( max-width: 1000px ) {
    div.main section {
      height: 360px;
      top: 20%;
    }
  }
  form {
    width: 220px;
    height: 240px;
    position: absolute;
    top: 40px;
    right: 15%;
  }
  .submit_btn {
    width: 100%;
  }
  .main >section > img {
    width: 338px;
    height: 70px;
    margin-top: 75px;
    margin-left: -30%;
  }
  @media (max-width: 1000px) {
    div.main > section > img {
      position: absolute;
      margin: auto;
      left: 0;
      right: 0;
      top: 10%;
    }
  }
  @media (max-width: 1000px)
  {
    div.main > section > form {
      margin: 0 auto;
      right: 0;
      left: 0;
      top: 40%;
    }
  }
  .el-input__inner {
    background-image: url("../images/login/user.png");
    padding: 0 15px 0 35px;
    background-repeat: no-repeat;
  }
  .people {
    background-image: url("../images/login/user.png");
    display: block;
    width: 20px;
    height: 20px;
    margin: 5px 0 0 10px;
    background-repeat: no-repeat;
    background-size: contain;
    position: absolute;
    top: 3px;
  }
  .pass {
    background-image: url("../images/login/pwd.png");
    display: block;
    width: 20px;
    height: 20px;
    margin: 5px 0 0 10px;
    background-repeat: no-repeat;
    background-size: contain;
    position: absolute;
    top: 55px;
  }
  .form-control {
    padding-left: 38px;
  }
  .form-group {
    margin-bottom: 20px;
  }
  .mbtn {
    margin-top: 10px;
    letter-spacing: 1px;
    font-size: 18px;
  }
  button {
    font-size: 16px;
  }
</style>
