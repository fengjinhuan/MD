<template>
<div id="demo-toobar">
    <div class="demo-top">
            <div class="toobar" ref="box">
                <div class="backs" @click="back">
                    <span></span>
                </div>
                <div class="more">
                    <span></span>
                </div>
            </div>
            <div class="img">
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
        back(){
            this.$router.push({ path: '/Demo' })
        }
    },
}
</script>
<style scoped>
.demo-top {
    height: 2.5rem;
    width: 100%;
    position: relative;
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
</style>