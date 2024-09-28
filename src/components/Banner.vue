<script>
  // Import Swiper Vue.js components
  import { Swiper, SwiperSlide } from 'swiper/vue';

  // Import Swiper styles
  import 'swiper/css';

  import 'swiper/css/pagination';

  
  // import required modules
  import {  Pagination } from 'swiper/modules';
  import {bannerdata} from './../data/Banner.js';

  import './../swiper/style.css';


  export default {
    components: {
      Swiper,
      SwiperSlide,
    },
    setup() {
      return {
        pagination: {
          clickable: true,
          renderBullet: function (index, className) {
            const SlideNames = ['Advent, EC CFD Case Study','Amazon HQ2 Case Study','New Nederland Office','ECS Company Acquisition','Environmental Changes Via Squid'];
            return '<span class="' + className + '">' + SlideNames[index] + '</span>';
          },
        },
        modules: [Pagination],
      };
    },
    data() {
        return {
            bannerdata
        }
    }
  };
</script>

<template>
  <swiper :pagination="pagination" :modules="modules" class="mySwiper">
    <swiper-slide v-for="bd in bannerdata" :key="bd.id">

        <div class="swiper-image" style="background-image: url(https://trinityprodblob2023.blob.core.windows.net/trinity-images-container/images/default-source/trinity/ls-images/case-study-feature/trinity-consultants-ensures-safe-airflow_feature-list.jpg?sfvrsn=9eac762d_1)">
            <div class="banner_content">
                <h2>
                    0{{bd.id}}<span> / 05</span>
                </h2>
                <h1 class="hero-carousel__title">{{bd.title}}</h1>

                    <a class="btn" href="`${bd.url}`" aria-label="Learn More">Learn More</a>
            </div>
            <div class="filter"></div>
        </div>

    </swiper-slide>

    

    <div class="swiper-pagination"></div>
    
  </swiper>
</template>