<template>
    <div class="temp">
        <!--图片轮播部分代码，从mint-ui组建中获取-->
        <mt-swipe :auto="4000">
            <mt-swipe-item class="slide2" v-for="(item,index) in lunboData" :key="index">
                {{ item.img }}
            </mt-swipe-item>
        </mt-swipe>
    </div>
</template>

<style scoped>
    .mint-swipe {
        height: 200px;
        color: #fff;
        font-size: 30px;
        text-align: center;
        margin-bottom: 20px;
    }

    .mint-swipe-item {
        line-height: 200px;
    }

    .slide1 {
        background-color: #0089dc;
        color: #fff;
    }

    .slide2 {
        background-color: #ffd705;
        color: #000;
    }

    .slide3 {
        background-color: #ff2d4b;
        color: #fff;
    }
</style>

<script type="text/ecmascript-6">
    export default {
        props:['lunboData']
    }
</script>