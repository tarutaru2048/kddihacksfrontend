<template>
    <v-app id="inspire">  
      <v-main>
  
        <v-container>
          <v-row>
            <v-col>
              <h1>2023年度  〇〇学会  Day2  会場3</h1>
            </v-col>
          </v-row>
          <v-row>
            <v-col
              v-for="card in cards"
              :key="card.title"
              cols="4"
            >

              <v-card class="mr-3" max-width="320" @click="navigateToChat(card.page)">
                <v-img
                  :src="card.image"
                  aspect-ratio="1.5"
                  contain
                  :style="{width: '100%', height: 'auto'}"
                ></v-img>
                <v-card-title class="text-wrap" style="line-height: 1.2; height: 3.0em; overflow: hidden;">{{card.title}}</v-card-title>
                <v-card-subtitle>{{card.subtitle}}</v-card-subtitle>
              </v-card>
              
            </v-col>
          </v-row>
        </v-container>
      </v-main>
    </v-app>
  </template>
  
  <script>
  import { useRouter } from 'vue-router';
  export default {
    name: 'HomePage',
    setup() {
    const router = useRouter();

    const navigateToChat = (page) => {
      router.push({ name: page });
    };

    return { navigateToChat };
    },
  
  
    data() {
    return {
      cards: [
        { title: '持続可能な開発目標における人工知能の影響の探究', subtitle: '田中太郎', image: '/images/wordcloud1.png' , page: 'chat1' },
        { title: 'クラウドコンピューティングセキュリティ：課題と緩和策', subtitle: '西川治郎', image: '/images/wordcloud2.png' , page: 'chat2' },
        { title: '研究3', subtitle: '研究者C', image: '/images/wordcloud1.png' , page: 'chat3' },
        { title: '研究4', subtitle: '研究者D', image: '/images/wordcloud2.png' , page: 'chat4' },
        { title: '研究5', subtitle: '研究者E', image: '/images/wordcloud1.png' , page: 'chat5' },
        { title: '研究6', subtitle: '研究者F', image: '/images/wordcloud2.png' , page: 'chat6' },
      ]
    }
  }
    
}
  
  
  </script>