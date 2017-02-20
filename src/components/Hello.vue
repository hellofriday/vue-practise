<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <h2>Essential Links</h2>

    <div>
      <div class="form-line">
        <span>邮箱：</span>
        <input type="text" name="email" placeholder="邮箱">
      </div>

      <div class="form-line">
        <span>手机号：</span>
        <input>
      </div>
      <div class="form-line">
        <span>用户名：</span>
        <input>
      </div>

      <div class="form-line">
        <span>密码：</span>
        <input>
      </div>

      <div class="sign-in">注册</div>
    </div>


  </div>
</template>

<script>
export default {
  name: 'hello',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App',
      errors: ''
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

  .sign-in {
    width: 200px;
    padding:10px 10px;
    margin-right: auto;
    margin-left: auto;
    margin-top: 40px;
    text-align: center;
    font-size: 18px;
    color: #fff;
    background-color: #e87d0d;
    border-radius: 20px;
    transition: background-color 0.2s;
    cursor: pointer;
  }

  .sign-in:active {
    background-color: #b85e19;
  }

  .form-line {
    margin-right: auto;
    margin-left: auto;
    width: 400px;
    display: flex;
    justify-content: space-around;
    align-items: center;
    margin-top: 20px;
  }

  span {
   width: 80px;
   text-align: right;
   font-size: 18px;
   color: #0b97c4;
 }

  input {
    width: 200px;
    padding: 5px 10px;
    font-size: 18px;
    color: #999;
  }

</style>
