<template>
    <div ref="wrapper">
        <slot></slot>
    </div>
</template>
<script>
import BScroll from 'better-scroll'
export default {
    data(){
        return {
            wrapper:{}
        }
    },
    mounted(){
        setTimeout(()=>{
            this.init()
        },100)
    },
    methods:{
        init(){
            this.wrapper = new BScroll(this.$refs.wrapper,{click:true,probeType:3})
        }
    }
}
</script>