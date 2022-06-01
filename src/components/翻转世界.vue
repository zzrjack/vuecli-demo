<template lang="">
  <div>
    <h1>{{msg}}</h1>
    <button @click="btn">逆转世界</button>
  </div>
</template>
<script>
export default {
  data() {
    return {
      msg:"Hello,Vue"
    }
  },
  methods: {
    btn(){
      let arr=this.msg.split("")
      arr.reverse()
      console.log(arr)
      this.msg=arr.join("")
    }
  },
}
</script>
<style lang="">
  
</style>