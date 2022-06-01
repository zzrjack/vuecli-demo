<template lang="">
  <div>
    <p>当前购买数量:{{count}}</p>
    <button @click="addFn">+1</button>
    <button @click="addCountFn(5)">+5</button>
  </div>
</template>
<script>
export default {
  data() {
    return {
      count:1
    }
  },
  methods: {
    addFn(){
      this.count++
    },
    addCountFn(num){
      this.count=this.count+num
    }
  },
}
</script>
<style lang="">
  
</style>