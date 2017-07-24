<template>
<div id="demo-details">
    <div class="details">
            <div class="tip">
                <h1 class="title">项目详情</h1>
                <div class="support">
                    <span>查看更多</span>
                    <span class="agree"></span>
                </div>
            </div>
            <p>这次众筹，有即将于那是极好的，那是极好的，那是极好的那是极好的那是极好的，那是极好的。</p>
        </div>
        <div class="details">
            <div class="tip line">
                <h1 class="title">更新10</h1>
                <div class="support">
                    <span>查看更多</span>
                    <span class="agree"></span>
                </div>
            </div>
            <div class="time">
                <span>第10次更新</span>
                <span>2017-01-22 22:44</span>
            </div>
            <h1 class="title">《隐龙传：影踪》独特中国风创新3D横版动作游戏</h1>
            <div class="int">
                <div class="int-name">
                    <span class="icon"></span>
                    <span>美格方互动</span>
                </div>
            </div>
    
            <p>这次众筹，有即将于那是极好的，那是极好的，那是极好的那是极好的那是极好的，那是极好的。</p>
        </div>
        <div class="details">
            <div class="tip">
                <h1 class="title">评论 238</h1>
            </div>
            <div class="comment">
                <div class="comment-top">
                    <div class="demo-main">
                        <div class="comment-icon"></div>
                        <div class="comment-main">
                            <h2 class="comment-name">钟sir.</h2>
                            <span class="comment-time">2017-01-22 22:44</span>
                        </div>
                    </div>
                    <div class="comment-cattle"></div>
                </div>
                <div class="comment-content">
                    <span class="comment-user">你好，能在电脑完美？</span>
                    <div class="comment-reply">
                        <h2 class="reply-name">官方</h2>
                        <span>回复</span>
                        <h2 class="reply-name">用户：</h2>
                        <span>有官方版本哦</span>
                    </div>
                </div>
            </div>
            <div class="comment">
                <div class="comment-top">
                    <div class="demo-main">
                        <div class="comment-icon"></div>
                        <div class="comment-main">
                            <h2 class="comment-name">钟sir.</h2>
                            <span class="comment-time">2017-01-22 22:44</span>
                        </div>
                    </div>
                    <div class="comment-cattle"></div>
                </div>
                <div class="comment-content">
                    <span class="comment-user">你好，能在电脑完美？</span>
                </div>
            </div>
            <div class="comment">
                <div class="comment-top">
                    <div class="demo-main">
                        <div class="comment-icon"></div>
                        <div class="comment-main">
                            <h2 class="comment-name">钟sir.</h2>
                            <span class="comment-time">2017-01-22 22:44</span>
                        </div>
                    </div>
                    <div class="comment-cattle"></div>
                </div>
                <div class="comment-content">
                    <span class="comment-user">你好，能在电脑完美？</span>
                    <div class="comment-reply">
                        <h2 class="reply-name">官方</h2>
                        <span>回复</span>
                        <h2 class="reply-name">用户：</h2>
                        <span>有官方版本哦</span>
                    </div>
                    <div class="comment-reply">
                        <h2 class="reply-name">用户</h2>
                        <span>回复</span>
                        <h2 class="reply-name">官方：</h2>
                        <span>谢谢</span>
                    </div>
                    <div class="comment-reply">
                        <h2 class="reply-name">用户</h2>
                        <span>回复</span>
                        <h2 class="reply-name">官方：</h2>
                        <span>很高兴见到你</span>
                    </div>
                    <div class="comment-reply" v-for="o in length">
                        <h2 class="reply-name">用户</h2>
                        <span>回复</span>
                        <h2 class="reply-name">官方：</h2>
                        <span>很高兴见到你</span>
                    </div>
                    <div class="support comment-reply md-center" @click="add">
                        <span>更多回复</span>
                        <span class="agree"></span>
                    </div>
                </div>
            </div>
        </div>
</div>
</template>
<script>
export default{
    data(){
        return{
            length:0,
        }
    },
    methods:{
        add(){
            this.length+=4;
        },
    },
}
</script>
<style scoped>
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
</style>