<template>
  <div id="app">
    <form @submit.prevent="submit">
      <label>
        <span>用户名</span>
        <input type="text" v-model="user.username">
      </label>
      <label>
        <span>密码</span>
        <input type="password" v-model="user.password">
      </label>
      <!-- <button>提交按钮</button> -->
      <input type="submit">
    </form>
  </div>
</template>
<script>
  export default {
    data(){
      return {
        user:{
          username: '',
          password: ''
        }
      }
    },
    methods:{
      submit(){
        console.log(this.user)
      }
    }
  }
</script>
<style scoped>

</style>