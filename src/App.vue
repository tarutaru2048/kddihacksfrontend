<template>
  <v-app>
    <v-app-bar
        app
      >
        <v-btn icon @click="$router.push('/')">
          <v-icon>mdi-home</v-icon>
        </v-btn>
        <v-toolbar-title>Chat-Cloud(アプリ名)</v-toolbar-title>
  
      </v-app-bar>
    <v-main>
      <router-view/>
    </v-main>
  </v-app>
</template>

<script>

export default {
  name: 'App',

  data: () => ({
    //
  }),
}
</script>
