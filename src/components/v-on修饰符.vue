<template lang="">
  <div @click="fatherFn">
    <p @click.stop="oneFn">.stop-阻止事件冒泡</p>
    <a href="https://www.baidu.com/" @click.prevent.stop>跳转百度</a>
    <p @click.once="twoFn">点击观察事件处理函数执行几次</p>  
  </div>
</template>
<script>
export default {
  methods: {
    fatherFn(){
      console.log("fatherFn")
    },
    oneFn(){
      console.log("P标签点击")
    },
    twoFn(){
      console.log("p标签被点击了")
    }
  },
}
</script>
<style lang="">
  
</style>