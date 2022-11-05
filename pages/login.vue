<template>
  <div class="background">
    <div class="modal">
      <h1>ĐĂNG NHẬP</h1>
      <label for="username"> Username </label
      ><input type="text" v-model="userName" id="username" />
      <label for="password"></label>Password
      <input type="password" v-model="password" id="password" />
      <button>ĐĂNG NHẬP</button>
      <div class="line">
        <span>Hoặc</span>
      </div>
      <div class="others">
        <div>Login with Google</div>
        <div>Login with Facebook</div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'LoginPage',
  layouts: 'fullComponent',
  data() {
    return { userName: '', password: '' }
  },
}
</script>
<style scoped>
.background {
  background: #f9fafb;
  height: 100vh;
  padding-top: 130px;
}
h1 {
  font-size: 30px;
  font-weight: 700;
  margin-bottom: 20px;
}

.modal {
  padding: 50px;
  height: 80%;
  width: fit-content;
  background: #fff;
  margin: auto;
  border-radius: 10px;
  box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 29px 0px;
}
input {
  border: 1px solid #333;
  border-radius: 5px;
  width: 500px;
  height: 40px;
  display: block;
  margin-bottom: 20px;
}
.line {
  border-bottom: 1px solid #333;
  width: 100%;
  position: relative;
  margin-bottom: 30px;
  margin-top: 50px;
}
.line span {
  position: absolute;
  top: -13px;
  left: calc(50% - 32px);
  background: #fff;
  padding: 0px 8px;
}
button {
  background: #093aec;
  color: #fff;
  padding: 6px 16px;
  border-radius: 4px;
  font-weight: 700;
}
</style>
