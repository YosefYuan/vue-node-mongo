<template>
  <div>
    这是商品列表页面  
    <span>{{$route.params.goodsId}}</span>    
    <span>{{$route.params.name}}</span>    
  </div>
</template>
<style>
    
</style>
<script>
export default {
  data(){
      return {
          msg:'hello vue'
      }
  }
}
</script>


