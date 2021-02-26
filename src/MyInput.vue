<template>
  <div class="red wrapper">
    <!-- <input type="text" :value="valueF" @input="$emit('inputZ', $event.target.value)" /> -->

    <input type="text" :value="value" @input="$emit('input', $event.target.value)" />
  </div>
</template>
<script>
  export default {
    name: "MyInput",
    props:{
      // valueF:{
        
      value:{
        type:String,
      }
    },
  }
</script>
<style scoped>
  .red{
    border: 2px solid red;
  }
  .wrapper{
    display: inline;
  }
  .red input {
    outline: none;
    border: none
  }
</style>