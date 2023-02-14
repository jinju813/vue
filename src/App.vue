<template>
  <div id="app">
    
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <MyLogin></MyLogin>
    
    <Signup></Signup>
    <MyPage></MyPage>
    <MyPage2></MyPage2>
  </div>
</template>

<script>
import MyLogin from './components/MyLogin.vue'
import Signup from './components/Signup.vue'
import MyPage from './components/MyPage.vue'
import MyPage2 from './components/MyPage2.vue'

export default {
  name: 'App',
  components: {
    MyLogin,
    Signup,
    MyPage,MyPage2

  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
