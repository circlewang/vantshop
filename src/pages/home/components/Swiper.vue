<template>
    <div class="heade-swiper">
           <van-swipe :autoplay="3000" indicator-color="white">
                <van-swipe-item v-for="img in images" :key="img.id">
                    <img class="swiper-img" :src="img.imgUrl">
                </van-swipe-item>
            </van-swipe>
        </div>
</template>

<script>
export default {
    name:'HomeSwiper',
    data(){
        return{
            images:[{
                id:'0001',
                imgUrl:'http://gw.alicdn.com/imgextra/i2/102/O1CN01G1HpAO1CcksSgurzd_!!102-0-lubanu.jpg',
            },{
                id:'0002',
                imgUrl:'http://gw.alicdn.com/imgextra/i4/85/O1CN01NvawWk1CUy90Z2X7Q_!!85-0-luban.jpg',

            },{
                id:'0003',
                imgUrl: 'http://img.alicdn.com/simba/img/TB18voJihYaK1RjSZFnSuu80pXa.jpg_q50.jpg',
            },{
                id:'0004',
                imgUrl:'http://gw.alicdn.com/imgextra/i3/49/O1CN01j9ejXq1CETszE7wqr_!!49-0-lubanu.jpg',
            }]
        }
        
    }
}
</script>

<style lang="less" scoped>

.heade-swiper{
    overflow: hidden;
    width: 100%;
    height: 0;
    padding-bottom: 31.75%;
    .swiper-img{
        width: 100%;
    }
}
</style>
