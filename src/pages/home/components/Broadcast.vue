<template>
    <div>
        <back-big-height></back-big-height>
        <div class="title">
            <span class="title-content">淘宝直播</span>
        </div>
        <div class="item-wrapper">
            <div class="item-top">
                <div class="item-top-big">
                    <img src="http://img.alicdn.com/imgextra/i1/1266505025207716392/TB2OLLjiC0mpuFjSZPiXXbssVXa_!!0-dgshop.jpg">
                    <div class="back"></div>
                </div>
                <div class="item-top-small">
                    <img src="https://gw.alicdn.com/imgextra/i4/154/TB2HvWxeUvMR1JjSZPcXXc1tFXa_!!154-0-luban.jpg_200x200q85s150.jpg_.webp">
                    <div class="back"></div>
                </div>
            </div>
            <div class="item-bottom">
                <div class="item">
                    <img src="https://gw.alicdn.com/imgextra/i3/50/TB24YzzcRfM8KJjSZFhXXcRyFXa_!!50-0-luban.jpg_200x200q85s150.jpg_.webp">
                    <div class="item-title">
                        <p class="item-title-con">珠光宝气</p>
                        <p class="item-desc-con">玫瑰金锁骨链</p>
                    </div>
                </div>
                <div class="item">
                    <img src="https://gw.alicdn.com/imgextra/i3/50/TB24YzzcRfM8KJjSZFhXXcRyFXa_!!50-0-luban.jpg_200x200q85s150.jpg_.webp">
                    <div class="item-title">
                        <p class="item-title-con">珠光宝气</p>
                        <p class="item-desc-con">玫瑰金锁骨链</p>
                    </div>
                </div>
                <div class="item">
                    <img src="https://gw.alicdn.com/imgextra/i3/50/TB24YzzcRfM8KJjSZFhXXcRyFXa_!!50-0-luban.jpg_200x200q85s150.jpg_.webp">
                    <div class="item-title">
                        <p class="item-title-con">珠光宝气</p>
                        <p class="item-desc-con">玫瑰金锁骨链</p>
                    </div>
                </div>
            </div>
        </div>
        <back-height></back-height>
    </div>
</template>

<script>
import BackBigHeight from '@/common/backheight/BackBigHeight'
import BackHeight from '@/common/backheight/BackHeight'
export default {
    name:'HomeBroadcast',
    components:{BackBigHeight,BackHeight}
}
</script>

<style lang="less" scoped>
    .title{
        background: linear-gradient(to right, #f189b1 , #f3659b,#f3357d); 
        color:#fff;
        width: 2.1rem;
        height:.62rem;
        margin-top:-.2rem;
        border-top-right-radius: 1rem;
        border-bottom-right-radius: 1rem;
        text-align: center;
        font-size: .3rem;
        line-height: .6rem;
        z-index:999;
        position: relative;
        .title-content{
            padding:0 .15rem;
        }
    }
    .item-wrapper{
        margin-top: -.4rem;
        position: relative;
        width: 100%;
        z-index:98;
        .item-top{
            height:0;
            overflow: hidden;
            padding-bottom: 35%;
            width: 100%;
            .item-top-big{
                width: 65%;
                float: left;
                img{
                    width: 100%;
                }
                .back{
                    position: relative;
                    z-index: 99;
                    margin-top: -1.3rem;
                    height:1.3rem;
                    background: linear-gradient(to top,rgba(0,0,0,0.3),rgba(0,0,0,0.2),rgba(255,255,255,0.1));
                }
            }
            .item-top-small{
                width: 35%;
                float: left;
                img{
                    width: 100%;
                }
                .back{
                    position: relative;
                    z-index: 99;
                    margin-top: -1.3rem;
                    height:1.3rem;
                    background: linear-gradient(to top,rgba(0,0,0,0.4),rgba(0,0,0,0.3),rgba(0,0,0,0.01));
                }
            }
        }
        .item-bottom{
            height:0;
            overflow: hidden;
            padding-bottom: 47%;
            width: 100%;
            .item{
                width: 33.33%;
                float: left;
                img{
                    width: 100%;
                }
                .item-title{
                    background: #fff;
                    padding: .2rem 0 0 .2rem; 
                    .item-title-con{
                        color:#333;
                        letter-spacing: .02rem;
                    }
                    .item-desc-con{
                        color:#ccc;
                        font-size: .2rem;
                        line-height: .4rem;
                    }
                }
            }
        }
    }
</style>
