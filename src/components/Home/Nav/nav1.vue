<template>
  <div class="conter">
    <div class="All">
      <div class="img">
        <img src="../../../assets/QQ截图20200602094647.png" alt />
      </div>
      <div class="box">
        <div class="box1">路径</div>
        <div class="box2">训练营</div>
        <div class="box3">楼+</div>
        <div class="box4">会员</div>
        <div class="box5">社区▼</div>
      </div>
      <div class="ipt">
        <input type="text" placeholder="搜索 课程/问答" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "",
  props: {
    },
  components: {
    
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
  width: 1400px;
  height: 50px;
  position: relative;
}
.img {
  width: 200px;
  height: 200px;
  margin-left: 120px;
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
.box1 {
  width: 150px;
  height: 21px;
  left: 200px;
  top: 15px;
  margin-left: 10px;
  position: absolute;
  font-size: 21px;
  background-color: rgb(232,255,212);
}
.box2 {
  width: 150px;
  height: 21px;
  left: 200px;
  top: 15px;
  margin-left: 90px;
  position: absolute;
  font-size: 21px;
  background-color: rgb(232,255,212);
}
.box3 {
  width: 150px;
  height: 21px;
  left: 200px;
  top: 15px;
  margin-left: 190px;
  position: absolute;
  font-size: 21px;
  background-color: rgb(232,255,212);
}
.box4 {
  width: 150px;
  height: 21px;
  left: 200px;
  top: 15px;
  margin-left: 260px;
  position: absolute;
  font-size: 21px;
  background-color: rgb(232,255,212);
}
.box5 {
  width: 150px;
  height: 21px;
  left: 200px;
  top: 15px;
  margin-left: 360px;
  position: absolute;
  font-size: 21px;
  background-color: rgb(232,255,212);
}
.ipt {
  width: 150px;
  height: 50px;
  left: 200px;
  top: 15px;
  margin-left: 870px;
  position: absolute;
  font-size: 30px;
  background-color: rgb(232,255,212);
}
</style>