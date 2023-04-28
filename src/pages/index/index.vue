<template>
  <view class="content">
      <uni-data-select
        style="width: 100%"
        v-model="value"
        :localdata="range"
        @change="change"
      ></uni-data-select>
  </view>
  <view class="cardList"  >
    <uni-card :is-shadow="false" margin="16rpx" :border="false" style="border-bottom: 1px solid black">
      <text class="uni-h6">卡片组件通用来显示完整独立的一段信息，同时让用户理解他的作用。例如一篇文章的预览图、作者信息、时间等，卡片通常是更复杂和更详细信息的入口点。</text>
    </uni-card>
  </view>
</template>

<script setup>
import { ref } from 'vue'

const title = ref('data')
const range= [
  { value: 0, text: "篮球" },
  { value: 1, text: "足球" },
  { value: 2, text: "游泳" },
  { value: 2, text: "游泳" },
  { value: 2, text: "游泳" },
  { value: 2, text: "游泳" },
  { value: 2, text: "游泳" },
  { value: 2, text: "游泳" },
  { value: 2, text: "游泳" },
  { value: 2, text: "游泳" },
  { value: 2, text: "游泳" },
  { value: 2, text: "游泳" },
  { value: 2, text: "游泳" },
  { value: 2, text: "游泳" },
  { value: 2, text: "游泳" },
  { value: 2, text: "游泳" },
  { value: 2, text: "游泳" },
  { value: 2, text: "游泳" },
  { value: 2, text: "游泳" },
  { value: 2, text: "游泳" },
  { value: 2, text: "游泳" },
  { value: 2, text: "游泳" },
  { value: 2, text: "游泳" },
  { value: 2, text: "游泳" },
  { value: 2, text: "游泳" },
  { value: 2, text: "游泳" },
]

function change(e){
  console.log(e)
}
const value = ref()
</script>

<style>
.content {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  margin: 16rpx;
}
</style>
