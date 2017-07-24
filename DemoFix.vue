<template>
<div  id="demo-fix">
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
                <span class="fix-icon money"></span>
                <span>查看回报</span>
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
.money{
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