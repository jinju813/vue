<template>
    <div>
      <div>
        <img alt="logo" src="../assets/logo.png" style="margin-bottom: 50px; margin-top: 50px;"/>
        <div id="mylogin">
          <form @submit.prevent="fnLogin">
            <p>
              <input class="w3-input" name="user_id" placeholder="Enter your ID" v-model="user_id"><br>
            </p>
            <p>
              <input name="user_password" class="w3-input" placeholder="Enter your password" v-model="user_pw" type="password">
            </p>
            <p>
              <button type="submit" class="w3-button w3-round" style="background-color: #9beacd; margin-bottom: 70px;">Login</button>
            </p>
          </form>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  
  export default {
    data() {
      return {
        user_id: '',
        user_pw: ''
      }
    },
    methods: {
      fnLogin() {
        if (this.user_id === '') {
          alert('ID를 입력하세요.')
          return
        }
  
        if (this.user_pw === '') {
          alert('비밀번호를 입력하세요.')
          return
        }
  
        alert('로그인 되었습니다.')
      }
    }
  }
  </script>
  
  <style>
   @import "https://www.w3schools.com/w3css/4/w3.css";
  #mylogin {
    width: 500px;
    margin: auto;
  }

  </style>