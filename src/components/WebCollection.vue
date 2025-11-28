<script setup>
    console.log("WebCollection.vue加载成功")
</script>

<template>
    <div class="Web-Collection">
        <h3 style="text-align: center;color: black;font-weight: bolder;padding-top: 20px;">收藏の网站</h3>
        <div class="list">
            <a class="a1" href="https://www.sdut.edu.cn/">山东理工大学</a>
            <a class="a1" href="https://jsjxy.sdut.edu.cn/">计算机科学与技术学院</a>
            <a class="a1" href="https://ehall.sdut.edu.cn/new/ehall.html">信息门户</a>
            <a class="a1" href="http://211.64.28.123/jwglxt/xtgl/login_slogin.html">教务系统</a>
            <a class="a1" href="https://www.chsi.com.cn/">学信网</a>
            <a class="a1" href="https://www.lanzoui.com/">网盘</a>
            <a class="a1" href="https://picui.cn/">图床</a>
            <a class="a1" href="https://wyapi.toubiec.cn/">音乐</a>
            <a class="a1" href="https://peanutdl.com/zh">视频</a>
            <a class="a1" href="https://github.akams.cn/">Github加速下载</a>
            <a class="a1" href="https://www.doubao.com/chat/">豆包</a>
            <a class="a1" href="https://aistudio.google.com/">Gemini</a>

        </div>
    </div>
</template>

<style scoped>
.a1{
    display: flex; 
    border-radius: 10px;
    width: 100%;
    text-align: center;
    align-items: center;
    justify-content: center;
    background-color:rgba(230, 230, 230, 0.75);
    color: black;
}

.Web-Collection {
    flex: 3;
    background-color: rgba(255, 255, 255, 0.7);
    padding: 20px;
    border-radius: 8px;
}

.list {
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
    padding: 10px;
}

.list a {
    flex: 0 0 calc(20% - 10px);
    box-sizing: border-box;
    padding: 10px 0;
    text-decoration: none;
}

.Web-Collection:hover,
.a1:hover{
    transform: scale(1.03);
    transition: transform 0.3s ease;
}
</style>