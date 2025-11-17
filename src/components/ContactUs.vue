<script setup>
    console.log("ContactUs.vue加载成功")
</script>

<template>
    <div class="Contact-Us">
        <a href="https://qm.qq.com/q/iD4238wPE6"><img class="img1" src="/src/img/QQ.png" alt="QQ"></a>
        <a href="mailto:pigeons2023@hotmail.com"><img class="img1" src="/src/img/email.png" alt="邮箱"></a>
        <a href="https://space.bilibili.com/627097633"><img class="img1" src="/src/img/bilibili.png" alt="Bilibili"></a>
        <a href="https://github.com/pigeons2023"><img class="img1" src="/src/img/github.png" alt="Github"></a>
    </div>
</template>

<style scoped>
.Contact-Us {
    flex: 1;
    background-color: rgba(255, 255, 255, 0.7);
    padding: 15px;
    border-radius: 8px;
    display: flex;
    align-items: center;
    justify-content: center;
}

.img1{
    width:30px;
    margin: 10px;
}

.Contact-Us:hover, 
.img1:hover{
    transform: scale(1.03);
    transition: transform 0.3s ease;
}
</style>