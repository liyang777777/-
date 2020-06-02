<template>
 <div>
   <Nav></Nav>
   <top1></top1>
 </div>
</template>
<script>
//头部 
import Nav from '../components/Home/Nav/Nav'
//全部课程
import top1 from '../components/Home/Top/top1'
 export default {
   name: '',
   props: {
   },
   components: {
     //引入组件
     Nav,
     top1
   },
   data () {
     return {

     }
   },
   methods: {

   },
   mounted() {

   },
   watch: {

   },
   computed: {

   }
 }
</script>

<style scoped lang='scss'>

</style>