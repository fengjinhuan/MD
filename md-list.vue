<template>
<div id="md-list">
    <div class="list" v-for="o in 20" @click="mdList">
        <img src="../assets/list.png" alt="">
        <div class="title">
            <h1>《隐龙传：影踪》独特中国风创新3D横版动作游戏</h1>
            <span>by 美格方互动</span>
        </div>
        <div class="subtitle">
            <span class="money">已筹 ￥3,434,242,92</span>
            <span class="line">·</span>
            <span class="progress">进度340.85%</span>     
        </div> 
    </div>
</div>
</template>
<script>
export default{
    data(){
        return{

        }
    },
    methods:{
        mdList(){
            this.$router.push({ path: '/DemoList' })
        }
    },
}
</script>
<style scoped>
#md-list{
    background: #fff;
    margin-bottom: 0.6rem;
}
.list{
    height: auto;width: 100%;
}
.list img{
    height: 1.42rem;width: 100%;
}
.title{
    padding: 0 0.1rem;
    box-sizing: border-box;
}
.subtitle{
    display: flex;
    padding: 0 0.1rem;
    box-sizing: border-box;
}
.list h1{
    display: inline;
    font-size: 0.16rem;
    line-height: 0.28rem;
}
.list span{
    font-size: 0.14rem;
    color: #959A9F;
    
}
.line{
    font-size: 0.2rem;
    font-weight: bold;
    color: #A7AAA5;
    margin: 0 0.08rem;
}
.subtitle{
    line-height: 0.4rem;
    margin-bottom: 0.1rem;
}
</style>