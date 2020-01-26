<template>
  <v-app>
    <v-content>
      <header>
        <v-container>
          <img alt="Tellerup FanKlub" src="@/assets/logo_withmargin.svg" />
        </v-container>
      </header>
      <v-toolbar>
        <v-toolbar-items class="container">
          <v-btn text>Tellerup FanKlub</v-btn>
          <v-btn text>Forum</v-btn>
          <v-btn text>Events</v-btn>
          <v-btn tile color="primary">Nyheder</v-btn>
          <v-btn text>Om Klubben</v-btn>
        </v-toolbar-items>
      </v-toolbar>
      <v-container>
        <v-row>
          <v-col cols="10">
            <router-view />
          </v-col>
          <v-col cols="2">
            <UserCard />
          </v-col>
        </v-row>
      </v-container>
    </v-content>
  </v-app>
</template>

<script>
import UserCard from "./components/UserCard";

export default {
  name: "App",

  data: () => ({
    //
  }),

  components: {
    UserCard
  }
};
</script>

<style lang="less">
header {
  background-color: #9c27b0;
}

.v-toolbar__items.container {
  padding: 0;
}
</style>
