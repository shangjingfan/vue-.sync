<template>
  <div>
    <!-- <MyInput :valueF="value" @inputZ="value = $event"/> -->

    <MyInput :value="value" @input="value = $event"/>
    <MyInput v-model="value" />

    <span>{{value}}</span>
    <button @click="value = 'frank'">修改value1</button>
    <!-- <hr /> -->

    <!-- <input type="text" :value="xxx" @input="xxx = $event.target.value" />
    <input type="text" v-model="xxx" />
    --- {{xxx}}
    <button @click="xxx='张三'">修改username</button> -->
  </div>
</template>
<script>
import MyInput from './MyInput.vue'
  export default {
    name: "App",
    components:{MyInput},
    data(){
      return {
        value: "123",
        // xxx: ""
      }
    },
  }
</script>
<style scoped>

</style>