<template>
    <div>
        <home-header></home-header>
        <home-swiper></home-swiper>
        <home-category></home-category>
        <home-hot></home-hot>
        <home-broadcast></home-broadcast>
        <home-like></home-like>
        <back-footer-height></back-footer-height>
        <common-footer></common-footer>
    </div>
</template>

<script>
import HomeHeader from './components/Header'
import HomeSwiper from './components/Swiper'
import HomeCategory from './components/Category'
import HomeHot from './components/Hot'
import HomeBroadcast from './components/Broadcast'
import HomeLike from './components/Like'
import CommonFooter from '@/pages/footer/Footer'
import BackFooterHeight from '@/common/backheight/BackFooterHeight'
export default {
    name:'Home',
    components:{HomeHeader,HomeSwiper,HomeCategory,HomeHot,HomeBroadcast,HomeLike,CommonFooter,BackFooterHeight}
};
</script>

<style lang="less" scoped>
</style>
