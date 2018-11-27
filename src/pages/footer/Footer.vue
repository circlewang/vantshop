<template>
    <div>
        <div class="footer">
            <div class="item">
                <span class="iconfont icon-size">&#xe6bb;</span>
                <p class="item-title">首页</p>
            </div>
            <div class="item">
                <span class="iconfont icon-size">&#xe671;</span>
                <p class="item-title">物流</p>
            </div>
            <div class="item">
                <span class="iconfont icon-size">&#xe6af;</span>
                <p class="item-title">购物车</p>
            </div>
            <div class="item">
                <span class="iconfont icon-size">&#xe684;</span>
                <p class="item-title">更多</p>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name:'Footer',
}
</script>

<style lang="less" scoped>
.footer{
    z-index:1000;
    position: fixed;
    bottom: 0;
    left:0;
    right:0;
    height:1rem;
    background-color: #fff;
    display: flex;
    .item{
        flex:1;
        text-align: center;
        .icon-size{
            font-size: .5rem;
            color:#555;
            line-height: .7rem;
        }
        .item-title{
            font-size: .2rem;
            color:#555;
            line-height: .2rem;
        }
    }
}
</style>
