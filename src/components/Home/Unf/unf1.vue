<template>
 <div class="conter">
   <div class="box">楼+实战课程 | 定期开班，导师助教全程辅导，最快最优成长</div>
   <div class="box1">更多></div>
   <div class="btn">
     <div v-for="(item,index) in list" :key="index">
      <div>{{item.name}}</div>
      <div>{{item.tags[0].name}}</div>
      <div>{{item.tags[1].name}}</div>
     </div>
   </div>
   <unf2></unf2>
 </div>
</template>

<script>
import axios from 'axios'
import unf2 from '../Unf/unf2'
 export default {
   name: '',
   props: {
   },
   components: {
     unf2
   },
   data () {
     return {
       list: [],
     }
   },
   methods: {
     getData() {
       axios.get('http://120.78.14.107/api/v2/index/louplus').then(res => {
         console.log(res.data);
         this.list = res.data
       }).catch(err => {
         console.log(err);
       })
     }
   },
   mounted() {
     this.getData()
   },
   watch: {

   },
   computed: {

   }
 }
</script>

<style scoped lang='scss'>
.conter {
  width: 1400;
  height: 400px;
  background: aquamarine;
  display: flex;
}
.box {
  width: 550px;
  height: 100px;
  display: flex;
  font-size: 20px;
  margin-left: 120px;
  margin-top: 35px;
}
.box1 {
  display: flex;
  font-size: 20px;
  margin-left: 600px;
  margin-top: 40px;
}
</style>
