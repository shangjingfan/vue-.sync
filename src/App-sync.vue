<template>
  <div id="app">
    父亲现在有{{total}}
    <hr />
    <Child :money=total v-on:update:money="total = $event"/>
    <!-- <Child :money.sync=total /> -->
  </div>
</template>

<script>
import Child from "./Child.vue"
export default {
  name: 'App',
  data(){
    return{
      total: 10000
    }
  },
  components: {
    Child
  }
}
</script>

<style lang="scss">

</style>
