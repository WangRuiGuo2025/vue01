<script setup>
    console.log("Headers.vue加载成功")
    function sleep(ms) {
        return new Promise(resolve => setTimeout(resolve, ms));
    }
    function search(){
        const searchinput = document.querySelector('.search-input').value.trim();
        if (searchinput === null || searchinput === '') {
            alert('请输入搜索内容');
        }else{
            console.log("搜索内容:%s",searchinput);
            sleep(600).then(()=>location.reload());
        }
    }
</script>

<template>
    <div class="top">
        <div class="Top-Contents">
            <div class="logo">
                <span id="span1">王瑞国的小站</span>
            </div>
            <div class="Navigation">
                <span id="span2"><a class="a2" href="#">首页</a></span>
                <span id="span3"><a class="a2" href="log-in.html">登录</a></span>
                <span id="span4"><a class="a2" href="register.html">注册</a></span>
            </div>
            <div class="Search">
                <input type="text" class="search-input" placeholder="输入内容以查询">
                <a class="a3" @click="search()"><img src="/src/img/search.png" alt="搜索" class="Search-Img"></a>
            </div>

        </div>
    </div>
</template>

<style scoped>
.top{
    width: 100%;
    height: 60px;
    line-height: 60px;
    background-color: rgba(0, 144, 172, 0.75);
    margin-bottom: 25px;
}

.Top-Contents{
    margin-right: 20px;
    padding-left: 20px;
    padding-right: 20px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 100%;
}

.search-input{
    width: 150px;
    height: 30px;
    padding: 5px;
    border-radius: 20px;
    text-align: center;
}

.Search-Img{
    width: 30px;
    height: 30px;
    text-align: center;
    vertical-align: middle;
}

.Navigation{
    text-align: center;
    display: flex;
    gap: 50px;
}

.a3:hover,
.Search-Img:hover{
    transform: scale(1.03);
    transition: transform 0.3s ease;
}
#span1{
    color: black;
    font-size:large;
    font-weight: bold;
}

#span2{
    margin-left: 0px;
    margin-right:0px;
}

#span3{
    margin-right: 0px;
}

#span4{
    margin-right:0px;
}

.body {
    display: flex;
    gap: 20px;
    padding: 0 20px;
    margin: 50px;
}
</style>