<script setup>
import ContactUs from './components/ContactUs.vue';
import Curtain from './components/Curtain.vue';
import Footers from './components/Footers.vue';
import Headers from './components/Headers.vue';
import Hitokoto from './components/Hitokoto.vue';
import Introduction from './components/Introduction.vue';
import WebCollection from './components/WebCollection.vue';
console.log("App.vue加载成功")
</script>

<template>
  <div class="background">
    <Curtain />
    <Headers />
    <div class="body">
      <div class="left-column">
        <Introduction />
        <ContactUs />
      </div>
      <div class="right-column">
        <Hitokoto />
        <WebCollection />
      </div>
      <div class="music">
        <iframe frameborder="no" border="0" marginwidth="0" marginheight="0" width="330" height="86" autoplay="1" src="http://music.163.com/outchain/player?type=2&id=1878807107&auto=1&height=66"></iframe>
      </div>
    </div>
    <Footers />
  </div>
</template>

<style scoped>
* {
  margin: 0;
  padding: 0;
}

.background {
  background-image: url(/src/img/bg.png);
  min-height: 100vh;
  min-width: 100vh;
  background-size: cover;
}

.body {
  display: flex;
  gap: 20px;
  padding: 0 20px;
  margin: 20px;
}

.left-column, .right-column {
    flex: 1;
    display: flex;
    flex-direction: column;
    gap: 15px;
}

.music{
    position: fixed;
    bottom: 30px;
    right: 30px; 
}
</style>