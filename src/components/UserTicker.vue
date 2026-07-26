<template>
  <div class="glass-card ticker-card">
    <div class="ticker-wrapper">
      <div v-for="(item, index) in tickerItems" :key="index" class="ticker-item">
        <span>{{ item.text }}</span>
        <span style="color: var(--success-color); font-weight: bold;">[生成完成]</span>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue';

const tickerItems = ref([
  {
    "text": "用户 138****3311 成功高价卖出九成新 iPad Pro 闲置"
  },
  {
    "text": "用户 189****6622 获得了搬家急售双门冰箱自提爆款文案"
  },
  {
    "text": "用户 131****9900 完成了奢侈品包包带发票保真实拍指南"
  },
  {
    "text": "用户 156****4455 生成了针对屠夫大刀砍价的高情商回复"
  },
  {
    "text": "用户 173****8811 取得了防到货恶意掉包申请退货防坑 SOP"
  }
]);
</script>
