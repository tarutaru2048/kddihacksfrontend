<template>
  <v-row justify="center">
    <v-col cols="5" class = "my-6">
    <h2>2023年度  〇〇学会  Day2  会場3</h2>
    <v-card class="pa-2 my-6">
    <v-card-title class="headline mb-0" style="white-space: pre-line;">
      持続可能な開発目標における人工知能の影響の探究
    </v-card-title>
    <v-card-subtitle class="subtitle-1">
      田中太郎
    </v-card-subtitle>
    <v-card-text>
      キーワード：
      <br>
      持続可能な開発目標
      <br>
      人工知能
      <br>
      AI（人工知能）
      <br>
      影響
      <br>
      テクノロジー
      <br>
      データ分析
    </v-card-text>
  </v-card>
    </v-col>
    <v-col cols="5">
      <ChatPage1 />
    </v-col>
  </v-row>
</template>

<script>
import { defineComponent } from 'vue';

// Components
import ChatPage1 from '@/components/ChatPage1.vue';

export default defineComponent({
  name: 'Chat1View',

  components: {
    ChatPage1,
  },
});
</script>