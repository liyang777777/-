<template>
 <div class="swiper-container">
     <swiper ref="mySwiper" :options = 'swiperOptions'>
         <swiper-slide v-for="(item,index) in pics" :key="index">
             <img src="item,picture_url" alt="">
         </swiper-slide>
         <div  class="swiper-pagination" slot="pagination"></div>
     </swiper>
     <div class="swiper-button-prev"></div>
     <div class="swiper-button-next"></div>
 </div>
</template> 
<script>
import {Swiper,SwiperSlide} from 'vue-awesome-swiper'
import 'swiper/css/swiper.css'
import axios from 'axios'
 export default {
   name: '',
   props: {
   },
   components: {
       Swiper,
       SwiperSlide
   },
   data () {
     return {
         pics: [],
         SwiperOptions: {
             pagination: {
                  el: '.swiper-pagination'
             },
            //  autoplay: true,
            navigation: {
                nextEl: 'swiper-button-next',
                prevEl: 'swiper-button-prev',
            },
            // Sone Swiper options/callback...
         }
     }
   },
   methods: {
        getData() {
            axios.get('http://120.78.14.107/api/v2/index/banner-pictures').then(res => {
                console.log(res.data);
                this.pics = res.data
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
.swiper-container {
    --swiper-theme-color: #ff6600;
    --swiper-navigation-color: #00ff33;
    --swiper-navigation-size: 130px;
}
.swiper-button-prev {
    left: 200px !important;
}
</style>