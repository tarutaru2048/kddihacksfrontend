<template>
  <v-row justify="center">
    <v-col cols="5" class = "my-6">
    <h2>2023年度  KDDIハッカソン学会  &nbsp; 会場:クサヤ温泉</h2>
    <v-card class="pa-2 my-6">
      <v-img
        src= "/images/economic.png"
        contain
        :style="{width: '100%', height: 'auto'}"
      ></v-img>
    <v-card-title class="headline mb-0" style="white-space: pre-line;">
      バングラディシュの貧困問題とマイクロクレジットの役割-ボグラ県のボイラ村とカシャハル村の調査を通じて-
    </v-card-title>
    <v-card-subtitle class="subtitle-1">
      MOHAMMAD ARMANUR RAHMAN
    </v-card-subtitle>
    <v-card-text>
      キーワード：
      <br>
      バングラディシュ
      <br>
      貧困問題
      <br>
      マイクロクレジット
      <br>
      NGO
      <br>
      農村開発
      <br>
      農業協同組合
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