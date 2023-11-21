<template>
  <div class="swiper-container">
    <div class="swiper-wrapper">
      <div class="swiper-slide" v-for="(card, index) in cards" :key="index">
        <div class="card">
          <img :src="card.image" alt="Card Image" class="card-image" />
          <div class="card-content">
            <h2>{{ card.title }}</h2>
            <p>{{ card.description }}</p>
          </div>
        </div>
      </div>
    </div>
    <div class="swiper-pagination"></div>
    <div class="swiper-button-next"></div>
    <div class="swiper-button-prev"></div>
  </div>
</template>

<script>
import Swiper from 'swiper';
import 'swiper/swiper-bundle.css';

export default {
  data() {
    return {
      cards: [
        {
          title: 'Card 1',
          description: 'Description for Card 1.',
          image: '/img/airbnb.png',
        },
        {
          title: 'Card 2',
          description: 'Description for Card 2.',
          image: '/img/google.png',
        },
        // Add more cards as needed
      ],
    };
  },
  // mounted() {
  //   const swiper = new Swiper('.swiper-container', {
  //     loop: true,
  //     pagination: {
  //       el: '.swiper-pagination',
  //       clickable: true,
  //     },
  //     navigation: {
  //       nextEl: '.swiper-button-next',
  //       prevEl: '.swiper-button-prev',
  //     },
  //   });
  // },
     grabCursor: true,
     pagination: {
        el: '.swiper-pagination',
        type: 'fraction',
      },
  
    formatFractionCurrent: function (number) {
      if (number < 10) {
        number = '0' + number;
      }
      return number;
    },
  
    renderFraction: function (currentClass, totalClass) {
        return '<span class="' + currentClass + '"></span>' +
                ' of' +
                '<span class="' + totalClass + '"></span>';
    },
    				

     navigation: {
        nextEl: '.swiper-button-next',
        prevEl: '.swiper-button-prev',
      },
  
};
</script>

<style scoped>
/* Add your component styling here */
.card {
  border: 1px solid #ddd;
  border-radius: 8px;
  overflow: hidden;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

.card-image {
  width: 100%;
  height: 200px;
  object-fit: cover;
}

.card-content {
  padding: 16px;
}

.swiper-container {
  width: 80%;
  margin: 0 auto;
}
</style>
