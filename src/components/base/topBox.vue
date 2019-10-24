<template>
    <div>
        <div class="top">
            <img src="@/assets/images/外综服企业列表/u336.png" alt="">
            <span>平台首页</span>
            <p>您好，<span>aaa</span><span>北京宜贸兴国际贸易有限公司</span><span>退出</span></p>
        </div>
    </div>
</template>
<script>
export default {
    
}
</script>
<style lang="scss" scoped>
@import '@/assets/css/rem.scss';
.top{
    color:#fff;
    font-size:14px;
    position: relative;
    border-width: 0px;
    // width: 100vw;
    height: 32px;
    // line-height: 32px;
    display: flex;
    justify-content: space-around;
    align-items: center;
    img{
        height: 100%;
        position: absolute;
        top:0;
        left:0;
        width: 100%;
        z-index:-1;
    }
    p{
        // color:#fff;
        span{
            margin-right:20px;
        }
    }
}  
</style>