<script setup>
    console.log("Hitokoto.vue加载成功")
    const hitokoto = () => {
        fetch('https://v1.hitokoto.cn')
            .then(response => response.json())
            .then(data => {
            const hitokoto = document.querySelector('#hitokoto_text')
            //hitokoto.href = `https://hitokoto.cn/?uuid=${data.uuid}`
            hitokoto.innerText = data.hitokoto
            })
            .catch(console.error)
            //官网用例
    }
    hitokoto()
</script>

<template>
    <div class="Hitokoto">
            <button type="button" class="btn" @click="hitokoto">刷新</button>
        <p id="hitokoto">
            <a href="#" id="hitokoto_text">:D 获取中...</a>
        </p>
    </div>
</template>

<style scoped>
.Hitokoto {
    flex: 1;
    flex-direction: column;
    background-color: rgba(255, 255, 255, 0.7);
    padding: 15px;
    border-radius: 8px;
    display: flex;
    align-items: center;
    justify-content: center;
    position: relative;
}

.btn {
    position: absolute;
    top: 15px;
    right: 15px;
    padding: 5px 10px;
    border: none;
    border-radius: 5px;
    cursor: pointer;
}

#hitokoto{
    color: black;
    text-decoration: none;
    font-weight: bold;
}

#hitokoto_text{
    color: black;
    text-decoration: none;
    font-weight: bold;
    
}

.Hitokoto:hover{
    transform: scale(1.03);
    transition: transform 0.3s ease;
}
</style>