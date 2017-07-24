<template>
<div class="" id="demo-content">
    <div class="content">
        <h1 class="title">《隐龙传：影踪》独特中国风创新3D横版动作游戏</h1>
        <div class="int">
            <div class="int-name">
                <span class="icon"></span>
                <span>美格方互动</span>
            </div>
            <div class="int-call">
                <span class="icon"></span>
                <span>私信</span>
            </div>
        </div>
        <div class="demo-line"></div>
        <div class="data">
            <div class="data-list">
                <h1 class="data-hover">￥98,523,62</h1>
                <span>已筹 192.18%</span>
            </div>
            <div class="data-list">
                <h1>￥523,62</h1>
                <span>目标金额</span>
            </div>
            <div class="data-list">
                <h1>29天</h1>
                <span>剩余时间</span>
            </div>
        </div>
        <div class="picture">
            <div class="people-box">
                <img src="../assets/peopleName.png" alt="" v-for="o in 6">
            </div>
            <div class="support">
                <span>186人支持</span>
                <span class="agree"></span>
            </div>
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
        
    },
}
</script>
<style scoped>
.content {
    padding: 0 0.15rem;
}

.title {
    font-size: 0.2rem;
    line-height: 0.24rem;
    margin: 0.18rem 0;
}

.int {
    height: 0.2rem;
    width: 100%;
    display: flex;
    justify-content: space-between;
}

.int-call {
    display: flex;
}

.int-name {
    display: flex;
}

.int-name .icon {
    margin-right: 0.1rem;
    height: 0.2rem;
    width: 0.2rem;
    background: url(../assets/name.png) center no-repeat;
}

.int-call .icon {
    margin-right: 0.1rem;
    height: 0.2rem;
    width: 0.2rem;
    background: url(../assets/call.png) center no-repeat;
}

.int span {
    font-size: 0.14rem;
    color: #565D66;
}

.demo-line {
    height: 0.06rem;
    width: 100%;
    margin: 0.25rem 0;
    background: url(../assets/line.png) center repeat-x;
}

.data {
    height: auto;
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: space-between;
}

.data-list {
    width: 33.33%;
    height: auto;
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    text-align: center;
}

.data-list h1 {
    font-size: 0.14rem;
    width: 100%;

    line-height: 0.24rem;
}

.data-list span {
    font-size: 0.12rem;
    color: #91969C;
    width: 100%;
    line-height: 0.22rem;
}

.data-hover {
    color: #31BBCB;
}

.picture {
    margin: 0.24rem 0;
    height: 0.32rem;
    width: 100%;
    display: flex;
    justify-content: space-between;
    line-height: 0.32rem;
}

.people-box {
    width: 2rem;
    height: 100%;
    overflow: hidden; 
}
.people-box img{
    height: 0.3rem;width: 0.3rem;
    box-sizing: border-box;
    border: 1px solid #fff;
    border-radius: 50%;
    overflow: hidden;
    margin-right: -0.08rem;
}
.support {
    display: flex;
    align-items: center;
}

.support span {
    font-size: 0.14rem;
    color: #6B7CA1;
}

.agree {
    margin-left: 0.05rem;
    height: 0.15rem;
    width: 0.15rem;
    background: url(../assets/agree.png) center no-repeat;
}
</style>