<script setup>
    console.log("Introduction.vue加载成功")
</script>

<template>
    <div class="Introduction">
        <div class="Basic-Information">
            <h3 style="text-align: center;color: black;font-weight: bolder;">基础信息</h3>
            <p class="p1"><span style="font-weight: bold;">姓名：</span>王瑞国</p>
            <p class="p1"><span style="font-weight: bold;">性别：</span>男</p>
            <p class="p1"><span style="font-weight: bold;">籍贯：</span>山东省邹城市</p>
            <p class="p1"><span style="font-weight: bold;">专业班级：</span>智能2501</p>
            <p class="p1"><span style="font-weight: bold;">学号：</span>25110570014</p>
        </div>
        <div class="Personal-Strengths">
            <h3 style="text-align: center;color: black;font-weight: bolder;">个人特长</h3>
            <ol>
                <li class ="li1">本人精通Office三件套的使用，能够制作出工整优良的文档、文稿。 </li>
                <li class ="li1">本人擅长使用PS、PR等专业软件，会制作短片、小视频、宣发传单等。 </li>
                <li class ="li1">本人擅长制作流程图，多维图表等，多维、立体化展示数据信息。 </li>
                <li class ="li1">本人了解基础C语言、Python编程，善于利用资源制作小程序提供更大方便。 </li>
                <li class ="li1">本人擅长运营B站、抖音账号，保持粉丝热度，善于捕获热点。 </li>
            </ol>
        </div>
    </div>
</template>

<style scoped>
.Introduction {
    flex: 3;
    background-color: rgba(255, 255, 255, 0.7);
    padding: 20px;
    border-radius: 8px;
}

.Basic-Information{
  padding: 40px;
}

.Personal-Strengths {
  padding: 20px;
}

.p1{
    color: black;
}

.li1{
    color: black;
    font-weight: normal;
}

.Introduction:hover{
    transform: scale(1.03);
    transition: transform 0.3s ease;
}
</style>