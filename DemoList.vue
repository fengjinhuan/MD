<template>
    <div class="demo-list">
        <demo-toobar></demo-toobar>
        <demo-content></demo-content>
        <demo-details></demo-details>
        <div class="demo-mb"></div>
        <div class="demo-fix">
            <div class="fix-box">
                <div class="fix-list">
                    <span class="fix-icon star"></span>
                    <span class="fix-num">5.4万</span>
                </div>
                <div class="fix-list">
                    <span class="fix-icon pen"></span>
                    <span class="fix-num">3200</span>
                </div>
            </div>
            <div class="demo-btn">
                <span class="fix-icon moneys"></span>
                <span>查看回报</span>
            </div>
        </div>
    </div>
</template>
<script>
import demoToobar from './DemoToobar.vue'
import demoContent from './DemoContent.vue'
import demoDetails from './DemoDetails.vue'
import demoFix from './DemoFix.vue'
export default{
    components:{ demoToobar , demoContent , demoDetails , demoFix },
    data(){
        return{
           
        }
    },
    methods:{
        
    },
   
}
</script>
<style>
.demo-mb{
    height: 0.44rem;width: 100%;
    background: #fff;
}
.line {
    border-bottom: 1px solid #eee;
}
.demo-top {  
    width: 100%;
}

.toobar {
    height: 0.3rem;
    width: 100%;
    padding: 0 0.1rem;
    box-sizing: border-box;
    display: flex;
    position: absolute;
    z-index: 99;
    left: 0;
    top: 0.35rem;
    justify-content: space-between;
    transition: all 0.1s;
}
.animate{
    top: 0;
    left: 0;
}
.toobar div {
    height: 0.3rem;
    width: 0.3rem;
    border-radius: 50%;
    background: #2D2D36;

    opacity: 0.7;
    display: flex;
    align-items: center;
    justify-content: center;
}


.more span {
    display: block;
    height: 0.16rem;
    width: 0.16rem;
}
.backs span {
    display: block;
    height: 0.16rem;
    width: 0.16rem;
}
.backs span {
    background: url(../assets/backs.png);
}

.more span {
    background: url(../assets/more.png) center no-repeat;
}

.img {
    height: 2.5rem;
    width: 100%;
    background: url(../assets/list.png) no-repeat;
    background-size: 100% 2.5rem;
}
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



.details {
    box-sizing: border-box;
    padding: 0 0.15rem;
    border-top: 0.1rem solid #F2F3F3;
}

.details p {
    line-height: 0.24rem;
    padding: 0.25rem 0;
    color: #697078;
}

.tip {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.time {
    width: 100%;
    line-height: 0.4rem;
    display: flex;
    align-items: center;
    justify-content: space-between;
}

.time span {
    color: #8690A0;
    font-size: 0.14rem;
}

.comment-top {
    width: 100%;
    height: 0.42rem;
    display: flex;
    justify-content: space-between;
    align-items: center;
    overflow: hidden;
}

.demo-main {
    display: flex;
    align-items: center;
    height: 100%;
}

.comment {
    margin-bottom: 0.22rem;
}

.comment-icon {
    height: 0.3rem;
    width: 0.3rem;
    background: url(../assets/peopleName.png) center no-repeat;
}

.comment-main {
    display: flex;
    flex-wrap: wrap;
    margin-left: 0.1rem;
}

.comment-cattle {
    height: 0.18rem;
    width: 0.18rem;
    background: url(../assets/cat.png) center no-repeat;
}

.comment-name {
    width: 100%;
    font-size: 0.14rem;
}

.comment-time {
    line-height: 0.24rem;
    width: 100%;
    font-size: 0.1rem;
    color: #AEB1B5;
}

.comment-content {

    display: flex;
    padding-left: 0.4rem;
    box-sizing: border-box;
    flex-wrap: wrap;
}

.comment-user {
    width: 100%;
    font-size: 0.16rem;
    margin: 0.2rem 0;
    line-height: 0.2rem;
}

.comment-reply {
    height: 0.38rem;
    width: 100%;
    background: #eee;
    font-size: 0.14rem;
    line-height: 0.22rem;
    display: flex;
    align-items: center;
}

.reply-name {
    font-size: 0.14rem;
    margin: 0 0.05rem;
}
.md-center{
    justify-content: center;
}
.demo-fix{
    position: fixed;
    left: 0;bottom: 0;
    height: 0.44rem;
    width: 100%;
    display: flex;
    background: #fff;

}
.fix-box{
    box-sizing: border-box;
    padding: 0.05rem 0 0 0.2rem;
    width: 50%;
    display: flex;
    height: 100%;
}
.fix-list{
    width: 50%;
    height: 100%;
    display: flex;
    justify-content: center;
}
.fix-icon{
    height: 0.17rem;width: 0.17rem;
}
.pen{
    background: url(../assets/pen.png) center no-repeat;
    align-self: center;
}
.star{
    background: url(../assets/star.png) center no-repeat;
    align-self: center;
}
.moneys{
    background: url(../assets/money.png) center no-repeat;
    align-self: center;
    margin-right: 0.05rem;
}
.fix-num{
    font-size: 0.08rem;
    margin-left: 0.05rem;
    color: #BCBFC3;
}
.demo-btn{
    width: 50%;
    height: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
    color: #fff;
    font-size: 0.14rem;
    background: #00D6A6;
}
</style>