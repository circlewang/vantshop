<template>
    <div>
        <div class="title">
            <span class="iconfont">&#xe600;</span>
            <span>猜你喜欢</span>
        </div>
        <div class="content">
            <div class="item-content">
                <div class="item-img-wrapper" v-for="like in likes" :key="like.id">
                    <img class="item-img" :src="like.imgUrl">
                    <div class="item-title">{{like.title}}</div>
                    <div class="item-cont">
                        <span class="icon-money">¥</span>
                        <span class="item-price">{{like.price}}</span>
                        
                        <span class="item-sold">{{like.slod}}人付款</span>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name:'HomeLike',
    data(){
        return{
            likes:[{
                id:'0001',
                imgUrl:"http://img.alicdn.com/bao/uploaded/i1/661967230/O1CN01zvIDuk23HO1xY9zAY_!!0-item_pic.jpg_300x300q85s150.jpg_.webp",
                title:"[为你推荐]多功能儿童双层床成人高低床子母上下床组合床实木饰面两层上下铺",
                price:'2380',
                slod:'6'
            },{
                id:'0002',
                imgUrl:"http://img.alicdn.com/bao/uploaded/i1/661967230/O1CN01zvIDuk23HO1xY9zAY_!!0-item_pic.jpg_300x300q85s150.jpg_.webp",
                title:"[为你推荐]多功能儿童双层床成人高低床子母上下床组合床实木饰面两层上下铺",
                price:'2380',
                slod:'6'
            },{
                id:'0003',
                imgUrl:"http://img.alicdn.com/bao/uploaded/i1/661967230/O1CN01zvIDuk23HO1xY9zAY_!!0-item_pic.jpg_300x300q85s150.jpg_.webp",
                title:"[为你推荐]多功能儿童双层床成人高低床子母上下床组合床实木饰面两层上下铺",
                price:'2380',
                slod:'6'
            },{
                id:'0004',
                imgUrl:"http://img.alicdn.com/bao/uploaded/i1/661967230/O1CN01zvIDuk23HO1xY9zAY_!!0-item_pic.jpg_300x300q85s150.jpg_.webp",
                title:"[为你推荐]多功能儿童双层床成人高低床子母上下床组合床实木饰面两层上下铺",
                price:'2380',
                slod:'6'
            },{
                id:'0005',
                imgUrl:"http://img.alicdn.com/bao/uploaded/i1/661967230/O1CN01zvIDuk23HO1xY9zAY_!!0-item_pic.jpg_300x300q85s150.jpg_.webp",
                title:"[为你推荐]多功能儿童双层床成人高低床子母上下床组合床实木饰面两层上下铺",
                price:'2380',
                slod:'6'
            },{
                id:'0006',
                imgUrl:"http://img.alicdn.com/bao/uploaded/i1/661967230/O1CN01zvIDuk23HO1xY9zAY_!!0-item_pic.jpg_300x300q85s150.jpg_.webp",
                title:"[为你推荐]多功能儿童双层床成人高低床子母上下床组合床实木饰面两层上下铺",
                price:'2380',
                slod:'6'
            }]
        }
    }
}
</script>

<style lang="less" scoped>
.title{
    text-align: center;
    color:red;
    padding: .2rem;
    font-size: .3rem;
}
.content{
    width: 100%;
    background-color: #f2f2f2;
    .item-content{
        width: 100%;
        display: flex;
        justify-content: space-around;
        flex-wrap: wrap;
        .item-img-wrapper{
            width: 48%;
            border-radius: .15rem;
            margin-bottom: .2rem;
            background: #fff;
            .item-img{
                width: 100%;
                border-top-right-radius: .15rem;
                border-top-left-radius: .15rem;
            }
            .item-title{
                line-height: .36rem;
                font-size: .2rem;
                letter-spacing: .01rem;
                margin:.15rem .2rem;
                box-sizing: border-box;
                text-overflow: -o-ellipsis-lastline;
                overflow: hidden;
                text-overflow: ellipsis;
                display: -webkit-box;
                -webkit-line-clamp: 2;
                line-clamp: 2;
                -webkit-box-orient: vertical;
                
            }
            .item-cont{
                padding: .2rem 0 .2rem .2rem;
                color:red;
                .icon-money{
                    font-size: .1rem; 
                }
                .item-price{
                    font-size: .35rem;
                }
                .item-sold{
                    float: right;
                    margin-right:.2rem;
                    font-size: .2rem;
                    color:#ccc;
                }
            }
        }
    }
}
</style>
