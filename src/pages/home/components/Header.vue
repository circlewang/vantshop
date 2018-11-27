<template>
    <div class="header">
        <div class="header-icon">
            <span class="iconfont icon-head">&#xe601;</span>
        </div>
        <div class="header-search">
            <span class="iconfont icon-search">&#xe600;</span>
            <span>寻找宝贝店铺</span>
        </div>
    </div>
</template>

<script>
export default {
    name:'HomeHeader',
}
</script>

<style lang="less" scoped>
.header{
    background: #f98736;
    color:#fff;
    height:.74rem;
    width: 100%;
    display: flex;
    .header-icon{
        display: inline-block;
        padding-left: .2rem;
        .icon-head{
            font-size: .7rem;
        }
    }
    .header-search{
        display: inline-block;
        flex: 1;
        font-size: .1rem;
        line-height: .11rem;
        border-radius:.1rem;
        text-align: center;
        padding: .2rem .5rem;
        margin:.1rem .2rem .1rem .1rem;
        background: #FF4E22;
        color:rgb(235, 233, 233);
        .icon-search{
            font-size: .28rem;
            margin-right: .05rem;
        }
    }
}
</style>

