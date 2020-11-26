<template>
  <v-app dark>
    <v-main class="mb-13" style="background-color: #1F2E35">
      <v-container>
        <nuxt />
      </v-container>
    </v-main>
    <v-footer
      padless
      fixed
      style="background-color: rgba(0,0,0,0);"
      >
      <v-row style="background-color: rgba(0,0,0,0);">
        <v-col cols="12" class="py-0">
          <v-bottom-navigation background-color="#2A3C44" color="#3DD598" style="border-radius: 12px 12px 0px 0px;">
            <v-btn value="chat-list" to="history">
        <v-icon icon>mdi-history</v-icon>
      </v-btn>
            <v-btn value="home" to="home">
        <v-icon>mdi-home</v-icon>
      </v-btn>
      <v-btn value="timeline" to="bookmark">
        <v-icon>mdi-bookmark-outline</v-icon>
      </v-btn>
    </v-bottom-navigation>
    </v-col>
      </v-row>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  data() {
    return {
      clipped: false,
      drawer: false,
      fixed: false,
      items: [
        {
          icon: "mdi-apps",
          title: "Welcome",
          to: "/"
        },
        {
          icon: "mdi-chart-bubble",
          title: "Inspire",
          to: "/inspire"
        }
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: "Vuetify.js"
    };
  }
};
</script>
