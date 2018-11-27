<template>
<div class="wrapper">
    <div class="radius"></div>
    <div class="category-content">
        <div class="item-category" v-for="category in categories" :key="category.id">
            <div class="item-img-wrapper">
                <img class="item-img" :src="category.imgUrl">
            </div>
            <div class="item-img-title">{{category.title}}</div>
        </div>
    </div>
    <back-height></back-height>
</div>
</template>

<script>
import BackHeight from '@/common/backheight/BackHeight'
export default {
    name:'HomeCategory',
    components:{BackHeight},
    data(){
        return{
            categories:[{
                id:'0001',
                title:'天猫',
                imgUrl:'https://gw.alicdn.com/tfs/TB1Wxi2trsrBKNjSZFpXXcXhFXa-183-144.png_.webp'
            },{
                id:'0002',
                title:'聚划算',
                imgUrl:'https://img.alicdn.com/tfs/TB10UHQaNjaK1RjSZKzXXXVwXXa-183-144.png?getAvatar=1_.webp'
            },{
                id:'0003',
                title:'天猫国际',
                imgUrl:'https://gw.alicdn.com/tfs/TB11rTqtj7nBKNjSZLeXXbxCFXa-183-144.png?getAvatar=1_.webp'
            },{
                id:'0004',
                title:'外卖',
                imgUrl:'https://gw.alicdn.com/tps/TB1eXc7PFXXXXb4XpXXXXXXXXXX-183-144.png?getAvatar=1_.webp'
            },{
                id:'0005',
                title:'天猫超市',
                imgUrl:'https://gw.alicdn.com/tfs/TB1IKqDtpooBKNjSZFPXXXa2XXa-183-144.png_.webp'
            },{
                id:'0006',
                title:'充值中心',
                imgUrl:'https://gw.alicdn.com/tfs/TB1o0FLtyMnBKNjSZFoXXbOSFXa-183-144.png_.webp'
            },{
                id:'0007',
                title:'飞猪旅行',
                imgUrl:'https://gw.alicdn.com/tfs/TB1ydXzhCzqK1RjSZPcXXbTepXa-183-144.png?getAvatar=1_.webp'
            },{
                id:'0008',
                title:'领金币',
                imgUrl:'https://gw.alicdn.com/tfs/TB1BqystrZnBKNjSZFrXXaRLFXa-183-144.png?getAvatar=1_.webp'
            },{
                id:'0009',
                title:'拍卖',
                imgUrl:'https://gw.alicdn.com/tfs/TB1CMf4tlnTBKNjSZPfXXbf1XXa-183-144.png?getAvatar=1_.webp'
            },{
                id:'00010',
                title:'分类',
                imgUrl:'https://gw.alicdn.com/tfs/TB18P98tyQnBKNjSZFmXXcApVXa-183-144.png?getAvatar=1_.webp'
            }]
        }
    }
}
</script>

<style lang="less" scoped>
    .radius{
        background-color: #fff;
        height:.4rem;
        border-radius: 50%;
        margin-top: -.19rem;
        z-index:999;
        position: relative;
    }
    .category-content{
        width: 100%;
        background: #fff;
        height:0;
        line-height: 3rem;
        padding-bottom: 50%;
        margin-top: -.25rem;
        border-top-right-radius: 50%;
        border-top-left-radius: 50%;
        position: relative;
        .item-category{
            float: left;
            overflow: hidden;
            position: relative;
            width: 20%;
            top:0;
            left:0;
            height:0;
            line-height: .5rem;
            padding-bottom: 23%;
            margin-top:.1rem;
            box-sizing: border-box;
            .item-img-wrapper{
                top:0;
                left:0;
                bottom:.1rem;
                padding: .11rem;
                box-sizing: border-box;
                .item-img{
                    width: 100%;
                }
            }
            .item-img-title{
                text-align: center;
                font-size: .18rem;
                color:#666;
            }
            
        }
    }


</style>

