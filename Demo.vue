<template>  
<div class="demo">
    <div class="demo-top">
        <header>
            <div class="demo-header">
                <h1 class="hot">推荐</h1>
                <h1 class="m-l">全部</h1>
            </div>
            <div class="search"></div>
        </header>
    </div>
    <md-nav></md-nav>
    <md-list></md-list>
</div>
</template>
<script>
import mdNav from './md-nav.vue'
import mdList from './md-list.vue'
export default{
    components:{ mdNav , mdList},
    data(){
        return{
        }
    },
    methods:{
        
    },
}
</script>
<style>


.demo{
    background: #fff;
}
header{
    height: 0.6rem;
    width: 100%;
    display: flex;
    line-height: 0.6rem;
    padding:0 0.2rem;
    box-sizing: border-box;
    align-items: center;
    justify-content: space-between;
}
.demo-header{
    display: flex;
}
header h1{
    font-size: 0.26rem;
    
}
.hot{
    color: #CBCDD0;
}
.m-l{
    margin-left: 0.2rem;
}
.search{
    height: 0.2rem;width: 0.2rem;
    background: url(../assets/search.png);
    
}

</style>