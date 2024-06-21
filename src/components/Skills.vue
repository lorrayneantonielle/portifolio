<template>
    <div class="container" ref="glideRef">
    <swiper
        ref="mySwiper"
        :slides-per-view="6"
        :space-between="50"
        @swiper="onSwiper"
        @slideChange="onSlideChange"
        :modules="modules" 
        :options="swiperOptions"
    >
        <swiper-slide>Slide 1</swiper-slide>
        <swiper-slide>Slide 2</swiper-slide>
        <swiper-slide>Slide 3</swiper-slide>
        <swiper-slide>Slide 4</swiper-slide>
        <swiper-slide>Slide 5</swiper-slide>
        <swiper-slide>Slide 6</swiper-slide>
        <swiper-slide>Slide 7</swiper-slide>
        <swiper-slide>Slide 8</swiper-slide>
        <swiper-slide>Slide 9</swiper-slide>
        <swiper-slide>Slide 10</swiper-slide>
        <swiper-slide>Slide 11</swiper-slide>
        <swiper-slide>Slide 12</swiper-slide>

        
    </swiper>
    </div>
</template>
<script>
import { Swiper, SwiperSlide } from 'swiper/vue';
import 'swiper/css';

export default {
    name: 'SoftHardSkills',
    components: {
        Swiper,
        SwiperSlide,
    },
    data() {
        return {
        swiperInstance: null,
        autoplayInterval: null,
        };
    },
    mounted() {
        this.startAutoplay();
    },
    beforeUnmount() {
        this.stopAutoplay();
    },
    methods: {
        onSwiper(swiper) {
        this.swiperInstance = swiper; 
        console.log('Swiper instance:', swiper);
        },
        onSlideChange() {
        console.log('Slide change');
        },
        startAutoplay() {
        this.autoplayInterval = setInterval(() => {
            if (this.swiperInstance) {
            this.swiperInstance.slideNext();
            }
        }, 3000);
        },
        stopAutoplay() {
        clearInterval(this.autoplayInterval);
        },
    },
};
</script>

<style scoped>
.container {
    padding:20px;
    max-width: 100%;
}
</style>