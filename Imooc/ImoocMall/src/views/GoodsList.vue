<template>
  <div>
    这是商品列表页面
    <span>{{$route.params.goodsId}}</span> <br>
    <span>{{$route.params.name}}</span>
    <router-link to="/goods/title">显示商品标题</router-link>
    <router-link to="/goods/image">显示商品图片</router-link>
    <div>
      <router-view></router-view>
    </div>
    <router-link :to="{name:'cart',params:{cartId:123}}">跳转到购物车页面</router-link>
  </div>
</template>
<style>

</style>
<script>
export default {
  data() {
    return {
      msg: 'hello vue'
    }
  },
  methods: { 
    jump () {
      this.$router.go(-2);
    }
  }
}
</script>


