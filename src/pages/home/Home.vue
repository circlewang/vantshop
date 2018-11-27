<template>
    <div>
        <home-header></home-header>
        <home-swiper></home-swiper>
        <home-category></home-category>
        <home-hot></home-hot>
    </div>
</template>

<script>
import HomeHeader from './components/Header'
import HomeSwiper from './components/Swiper'
import HomeCategory from './components/Category'
import HomeHot from './components/Hot'
export default {
    name:'Home',
    components:{HomeHeader,HomeSwiper,HomeCategory,HomeHot}
};
</script>

<style lang="less" scoped>
</style>
