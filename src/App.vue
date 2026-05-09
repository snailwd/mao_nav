<template>
  <!-- 自动滚动联系方式板块 -->
  <div class="auto-scroll-box">
    <div class="auto-scroll-list">
      <!-- 第一组内容 -->
      <div class="scroll-item">
        <div class="icon-box">💬</div>
        <div class="txt">旺旺782585521</div>
      </div>
      <div class="scroll-item">
        <div class="icon-box">🫧</div>
        <div class="txt">泡泡294236890</div>
      </div>
      <div class="scroll-item">
        <div class="icon-box">✈️</div>
        <div class="txt">飞机wy211111</div>
      </div>

      <!-- 无缝循环复制一遍 不用改 -->
      <div class="scroll-item">
        <div class="icon-box">💬</div>
        <div class="txt">旺旺782585521</div>
      </div>
      <div class="scroll-item">
        <div class="icon-box">🫧</div>
        <div class="txt">泡泡294236890</div>
      </div>
      <div class="scroll-item">
        <div class="icon-box">✈️</div>
        <div class="txt">飞机wy211111</div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.auto-scroll-box {
  width: 100%;
  overflow: hidden;
  padding: 18px 0;
  background: #ffffff;
  border-radius: 16px;
  margin: 15px 0;
}

.auto-scroll-list {
  display: flex;
  gap: 30px;
  animation: moveScroll 20s linear infinite;
}

/* 鼠标放上去暂停滚动 */
.auto-scroll-list:hover {
  animation-play-state: paused;
}

@keyframes moveScroll {
  0% { transform: translateX(0); }
  100% { transform: translateX(-50%); }
}

.scroll-item {
  flex-shrink: 0;
  text-align: center;
  width: 110px;
}

.icon-box {
  width: 56px;
  height: 56px;
  margin: 0 auto 8px;
  border-radius: 14px;
  background: #f0f4ff;
  font-size: 24px;
  display: flex;
  align-items: center;
  justify-content: center;
}

.txt {
  font-size: 14px;
  color: #333;
  white-space: nowrap;
}
</style>
