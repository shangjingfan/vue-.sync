<template>
  <div>
    儿子要花父亲的钱{{money}}
    <button @click="$emit('update:money', money - 100)">花钱</button>
  </div>
</template>
<script>
  export default {
    props:["money"]
  }
</script>
<style scoped>

</style>