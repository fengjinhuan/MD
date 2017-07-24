<template>
<div id="md-nav">
    <nav>
        <div class="demo-class" @click="sel">
            <div v-if="flag">{{def}}</div>
            <div class="color" v-else>{{def}}</div>
            <div class="demo-icon xia" v-if="flag"></div>
            <div class="demo-icon shang" v-else></div>
        </div>
        <div class="demo-class" @click="sel1">
            <div v-if="flag1">{{def1}}</div>
            <div class="color" v-else>{{def1}}</div>
            <div class="demo-icon xia" v-if="flag1"></div>
            <div class="demo-icon shang" v-else></div>
        </div>
        <div class="demo-class" @click="sel2">
            <div v-if="flag2">{{def2}}</div>
            <div class="color" v-else>{{def2}}</div>
            <div class="demo-icon xia" v-if="flag2"></div>
            <div class="demo-icon shang" v-else></div>
        </div>
    </nav>
    <div class="demo-list one" v-if="item">
            <div class="title" v-for="item in title" @click="itemSel">
                {{item}}
            </div>
            <div class="title color" v-if="itemDef">全部</div>
            <div class="title" v-else>全部</div>
    </div>
    <div class="demo-list two" v-if="item1">
            <div class="title1" v-for="item in title1" @click="itemSel1">
                <span>{{item}}</span>
                <div class="item1-icon"></div>
            </div> 
            <div class="title1 color" v-if="itemDef1">
                <span>全部状态</span>
                <div class="item1-icon dui"></div>
            </div>
            <div class="title1" v-else>
                <span>全部状态</span>
                <div class="item1-icon"></div>
            </div>
    </div>
    <div class="demo-list three" v-if="item2">
            <div class="title1" v-for="item in title2" @click="itemSel2">
                <span>{{item}}</span>
                <div class="item1-icon"></div>
            </div> 
            <div class="title1 color" v-if="itemDef1">
                <span>最新上线</span>
                <div class="item1-icon dui"></div>
            </div>
            <div class="title1" v-else>
                <span>最新上线</span>
                <div class="item1-icon"></div>
            </div>
    </div>
</div>
</template>
<script>
export default{
    data(){
        return{
            
            flag:true,
            flag1:true,
            flag2:true,
            item:false,
            item1:false,
            item2:false,
            itemDef:true,
            itemDef1:true,
            itemDef2:true,
            title:['游戏','动漫','出版','活动','音乐','影视','设计','科技'],
            title1:['创意','预热','众筹中','众筹成功'],
            title2:['金额最多','评论最多'],
            def:"全部",
            def1:"全部状态",
            def2:"最新上线",
        }
    },
    methods:{
        sel(){
            if(this.flag==true){
                
                this.flag=false;
                this.item=true;
                this.flag1=true;
                this.item1=false;
                this.flag2=true;
                this.item2=false;
            }else{
                
                this.flag=true;
                this.item=false;
            }    
        },
        sel1(){
            if(this.flag1==true){
                
                this.flag1=false;
                this.item1=true;
                this.flag=true;
                this.item=false;
                this.flag2=true;
                this.item2=false;
            }else{
                
                this.flag1=true;
                this.item1=false;
            }    
        },
        sel2(){
            if(this.flag2==true){
                
                this.flag2=false;
                this.item2=true;
                this.flag1=true;
                this.item1=false;
                this.flag=true;
                this.item=false;
            }else{
               
                this.flag2=true;
                this.item2=false;
            }    
        },
        
        itemSel:function(event){
            
            this.itemDef=false;
            event.target.className="title color"
            event.target.parentNode.className="demo-list one animate"
            console.log(event.target.parentNode.className)
            this.flag=true;
            this.def=event.target.innerHTML
            var _this=this;
            setTimeout(function() {
                _this.item=false;
            }, 300);
        },
        itemSel1:function(event){
            
            this.itemDef1=false;
            event.target.children[0].className="color"
            event.target.children[1].className="item1-icon dui"
            event.target.parentNode.className="demo-list two animate"  
            this.flag1=true;
            this.def1=event.target.children[0].innerHTML
            var _this=this;
            setTimeout(function() {
                _this.item1=false;
            }, 300);
        },
        itemSel2:function(event){
            
            this.itemDef2=false;
            event.target.children[0].className="color"
            event.target.children[1].className="item1-icon dui"
            event.target.parentNode.className="demo-list two animate"
            this.flag2=true;
            this.def2=event.target.children[0].innerHTML
            var _this=this;
            setTimeout(function() {
                _this.item2=false;
            }, 300);
        }
    },
}
</script>
<style scoped>

nav{
    min-height: 0.4rem;width: 100%;
    display: flex;
    justify-content: space-between;
    padding: 0 0.2rem;
    box-sizing: border-box;
    flex-wrap: wrap;
}
.demo-class{
    height: 0.4rem;
    width: auto;
    line-height: 0.4rem;
    display: flex;
    align-items: center;
}
.demo-icon{
    margin-left: 0.1rem;
    height: 0.12rem;
    width: 0.18rem;  
}
.xia{
    background: url(../assets/xia.png) no-repeat;
}
.shang{
    background: url(../assets/shang.png) no-repeat;
}

.demo-list{
    border-top: 1px solid #eee;
    width: 100%;
    font-size: 0.14rem; 
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    transition: all 0.3s;
}
.one{
    box-sizing: border-box;
}
.two{
    height: 2.4rem;
    padding: 0 0.2rem;
    box-sizing: border-box;
   
}
.three{
    height: 1.4rem;
    padding: 0 0.2rem;
    box-sizing: border-box;
    
}
.demo-list .title{
    width: 20%;
    
    font-size: 0.14rem;
    text-align: center;
}
.demo-list .title1{
    width: 100%;
    display: flex;
    justify-content: space-between;
}
.animate{
    height:0rem ;
    overflow: hidden;
}
.item1-icon{
    height: 0.18rem;
    width: 0.18rem;
    border: 1px solid #8C9197;
    text-align: center;
    border-radius: 50%;
    box-sizing: border-box;
}
.dui{
    border: none;
    background: url(../assets/dui.png) no-repeat;
    background-size: 0.18rem;
}














.color{
    color:#00CBB2;
}
</style>