<template>
    <div>
        <div class="content">
            <topBox></topBox>
            <logo></logo>
            <div class="loginBox">
                <div>
                    <span>账号：</span>
                    <input type="text">
                </div>
                <div>
                    <span>密码：</span>
                    <input type="password">
                </div>
                <div>
                    <button>登录</button>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
import topBox from '@/components/base/topBox'
import logo from '@/components/base/logo'
export default {
    components:{
        topBox,
        logo
    }
}
</script>
<style lang="scss" scoped>
   .content{
      
       .loginBox{
           padding: 40px;
           box-sizing: border-box;
           margin: 100px auto;
            width: 603px;
            height: 330px;
            background: rgb(242,242,242);
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: space-around;
            input{
                width: 300px;
                height: 36px;
            }
            button{
                width: 360px;
                height: 40px;
                background:rgba(22, 155, 213, 1);
                border-radius: 10px;
                border:0;
                outline: none;
                color:#fff;
            }
       }
   }
</style>