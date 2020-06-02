<template>
  <div class="conter">
    <div class="All">
      <div class="img">
        <img src="https://static.shiyanlou.com/frontend/dist/img/9f43b00.svg" alt="实验楼">
      </div>
      <div class="box">
        <div class="box1">做实验，学编程</div>
        <div class="box2">企业版|学校版</div>
        <div class="btn">
          <div class="btn1">登录</div>
          <div class="btn2">注册</div>
        </div>
      </div>
    </div>
    <nav1></nav1>
  </div>
</template>
<script>

import nav1 from '../Nav/nav1'
export default {
  name: "",
  props: {},
  components: {
    nav1
  },
  data() {
    return {
     
  }
  },
  methods: {
    
  },
  mounted() {},
  watch: {},
  computed: {}
}
</script>

<style scoped lang='scss'>

.All {
  width: 1000px;
  height: 50px;
  position: relative;
}
.img {
  width: 110px;
  height: 60px;
  margin-left: 100px;
}
.box {
  width: 150px;
  height: 21px;
  left: 200px;
  top: 9px;
  margin-left: 10px;
  position: absolute;
  font-size: 21px;
}
.box2 {
  width: 122px;
  height: 35px;
  left: 725px;
  top: 0px;
  position: absolute;
  font-size: 19px;
  background-color: rgb(8,191,145);
}
.btn {
  width: 186px;
  height: 68px;
  right: 50px;
  top: 30px;
  position: absolute;
  font-size: 18px;
  
}
.btn1 {
  width: 45px;
  height: 35px;
  margin-left: 960px;
  margin-top: -29px;
  position: absolute;
  font-size: 22px;
  background-color: rgb(8,191,145);
}
.btn2 {
  width: 80px;
  height: 50px;
  margin-left: 1030px;
  margin-top: -29px;
  position: absolute;
  font-size: 30px;
  background-color: rgb(8,191,145);
}
</style>