<script setup>
    console.log("Curtain.vue加载成功")
</script>

<template>
    <div class="curtain-container">
        <div class="left-curtain"></div>
        <div class="right-curtain"></div>
    </div>
</template>

<style scoped>
.curtain-container {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100vh;
    z-index: 1;
    pointer-events: none;
}

.left-curtain, .right-curtain {
    position: absolute;
    top: 0;
    height: 100vh;
    width: 50%;
    background-color: rgba(240, 240, 240, 0.9);
    animation: pullCurtain 1.2s cubic-bezier(0.645, 0.045, 0.355, 1) forwards;
}

.left-curtain {
    left: 0;
    transform-origin: left center;
}

.right-curtain {
    right: 0;
    transform-origin: right center;
}

@keyframes pullCurtain {
    0% {
        transform: scaleX(1);
    }
    100% {
        transform: scaleX(0);
    }
}

</style>