<template>
  <div id="Header">
    <div class="content-wrapper">
      <div class="icon">
        <img
          src="http://static.galileo.xiaojukeji.com/static/tms/seller_avatar_256px.jpg"
          width="64"
          height="64"
        >
      </div>
      <div class="content">
        <div class="tilte">
          <span class="logo"></span>
          <span class="name">曹氏大盘鸡</span>
        </div>
        <div class="description">蜂鸟专送/30分钟送达</div>
        <div class="support">
          <span class="icon decrease"></span>
          <span class="text">在线支付满28减5</span>
        </div>
      </div>
      <div class="supports-count" @click="Showdetail">
        <span>5个</span>
        <i class="layui-icon layui-icon-right"></i>
      </div>
    </div>
    <div class="bg">
      <img
        src="http://static.galileo.xiaojukeji.com/static/tms/seller_avatar_256px.jpg"
        width="100%"
        height="100%"
      >
    </div>
    <transition name="fade">
     <div v-show="isshow" class="detail">
      
    </div>
    </transition>
  </div>
</template>
<script>
export default {
  data(){
    return{
      isshow:false
    }
  },
  methods:{
    Showdetail(){
      this.isshow=true;
    }
  }
}
</script>
<style lang="stylus" rel="stylesheet/stylus">
@import 'header.styl';
</style>

