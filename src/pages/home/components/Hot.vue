<template>
    <div class="wrapper">
        <div class="item-content" v-for="hot in hots" :key="hot.id">
            <div class="item-img-content">
                <div class="item-title">{{hot.title}}</div>
                <p class="item-desc">{{hot.desc}}</p>
                <div class="item-img-wrapper1">
                    <img class="item-img" :src="hot.imgUrl1">
                </div>
            </div>
            <div class="item-img-wrapper2">
                <img class="item-img" :src="hot.imgUrl2">
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name:'HomeHot',
    data(){
        return{
            hots:[{
                id:'0001',
                title:'淘抢购',
                desc:'',
                imgUrl1:'http://gw.alicdn.com/imgextra/O1CN011C5JxZmejQVSexu_!!29-0-lubanu.jpg_100x100q85s150.jpg_.webp',
                imgUrl2:'http://gw.alicdn.com/imgextra/O1CN01TrgqTT1D6z0vz5u5J_!!168-0-lubanu.jpg_200x200q85s150.jpg_.webp'
            },{
                id:'0002',
                title:'有好货',
                desc:'高颜值美物',
                imgUrl1:'http://gw.alicdn.com/imgextra/O1CN011C5JxZmejQVSexu_!!29-0-lubanu.jpg_100x100q85s150.jpg_.webp',
                imgUrl2:'http://gw.alicdn.com/imgextra/O1CN01TrgqTT1D6z0vz5u5J_!!168-0-lubanu.jpg_200x200q85s150.jpg_.webp'
            },{
                id:'0003',
                title:'哇哦视频',
                desc:'2018流行啥',
                imgUrl1:'http://gw.alicdn.com/imgextra/O1CN011C5JxZmejQVSexu_!!29-0-lubanu.jpg_100x100q85s150.jpg_.webp',
                imgUrl2:'http://gw.alicdn.com/imgextra/O1CN01TrgqTT1D6z0vz5u5J_!!168-0-lubanu.jpg_200x200q85s150.jpg_.webp'
            },{
                id:'0004',
                title:'必买清单',
                desc:'购物全攻略',
                imgUrl1:'http://gw.alicdn.com/imgextra/O1CN011C5JxZmejQVSexu_!!29-0-lubanu.jpg_100x100q85s150.jpg_.webp',
                imgUrl2:'http://gw.alicdn.com/imgextra/O1CN01TrgqTT1D6z0vz5u5J_!!168-0-lubanu.jpg_200x200q85s150.jpg_.webp'
            }]
        }
    }
}
</script>

<style lang="less" scoped>
.wrapper{
    width: 100%;
    overflow: hidden;
    .item-content{
        width: 49%;
        height:0;
        padding-bottom: 35%;
        overflow: hidden;
        display: inline-block;
        .item-img-content{
            float: left;
            width: 49%;
             .item-title{
                display: inline-block;
                padding: .2rem 0 .1rem .3rem;
                box-sizing: border-box;
                font-size: .34rem;
            }
            .item-desc{
                font-size: .2rem;
                padding-left: .3rem;
                color:rgb(153, 153, 153);
                height:.25rem;
            }
            .item-img-wrapper1{
                width:100%;
                margin:0 .1rem 0 .1rem;
                padding: .15rem .2rem .2rem .2rem;
                box-sizing: border-box;
                .item-img{
                    width: 100%;
                    height:100%;
                    box-sizing: border-box;
                }
            }
        }
        .item-img-wrapper2{
            float: left;
            width: 50%;
            padding: .2rem .1rem 0 0;
            box-sizing: border-box;
            .item-img{
                width: 100%;
                height:100%;
                margin: .1rem .2rem 0 .1rem;
                padding: .1rem;
                box-sizing: border-box;
            }
        }
    }
}
</style>
