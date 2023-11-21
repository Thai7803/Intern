<template>
  <div class="swiper-container">
    <div class="swiper-wrapper">
      <div v-for="(slide, index) in slides" :key="index" class="swiper-slide">
        <img :src="slide.image" alt="Slide {{ index + 1 }}" />
        <p>{{ slide.caption }}</p>
      </div>
    </div>
    <div class="swiper-pagination"></div>
    <div class="swiper-button-next"></div>
    <div class="swiper-button-prev"></div>
  </div>
</template>

<script lang="ts">
import Swiper from 'swiper';
import 'swiper/swiper-bundle.css';

export default {
  data() {
    return {
      slides: [
        { image: '/img/airbnb.png', caption: 'Caption 1' },
        { image: '/img/amazon.png', caption: 'Caption 2' },
        // Thêm các slide khác nếu cần
      ],
    };
  },
  mounted() {
    // Khởi tạo Swiper khi component được mount
    new Swiper('.swiper-container', {
      // Cấu hình Swiper ở đây nếu cần
      navigation: {
        nextEl: '.swiper-button-next',
        prevEl: '.swiper-button-prev',
      },
      pagination: {
        el: '.swiper-pagination',
        clickable: true,
      },
    });
  },
};
</script>

<style scoped>
/* Thêm các quy tắc CSS cần thiết cho slideshow của bạn */
/* Ví dụ sử dụng Tailwind CSS classes */
.swiper-container {
  max-width: 600px;
  margin: 0 auto;
}

.swiper-slide img {
  width: 100%;
  height: auto;
}

.swiper-pagination-bullet {
  background-color: #007bff;
}
</style>
