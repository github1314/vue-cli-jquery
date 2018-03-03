<template>
  <div class="box">

  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
$(function () {
  $('.box').click(function () {
      console.log('我已经能成功使用jquery了')
  })
})
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .box{
    width: 100px;
    height: 100px;
    background-color:red;
  }
</style>
