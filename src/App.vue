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
          <v-col>
            <router-view />
          </v-col>
          <v-col>

            <v-card height="350px">
                <v-navigation-drawer
                  absolute
                  permanent
                  right
                >
                  <template v-slot:prepend>
                    <v-list-item two-line>
                      <v-list-item-avatar>
                        <img src="https://randomuser.me/api/portraits/women/63.jpg">
                      </v-list-item-avatar>

                      <v-list-item-content>
                        <v-list-item-title>Jane Smith</v-list-item-title>
                        <v-list-item-subtitle>Logged In</v-list-item-subtitle>
                      </v-list-item-content>
                    </v-list-item>
                  </template>

                  <v-divider></v-divider>

                  <v-list dense>

                    <v-list-item>
                      <v-list-item-icon>
                        <v-icon>mdi-home-city</v-icon>
                      </v-list-item-icon>
                      <v-list-item-content>
                        <v-list-item-title>Home</v-list-item-title>
                      </v-list-item-content>
                    </v-list-item>

                    <v-list-item>
                      <v-list-item-icon>
                        <v-icon>mdi-account</v-icon>
                      </v-list-item-icon>
                      <v-list-item-content>
                        <v-list-item-title>Account</v-list-item-title>
                      </v-list-item-content>
                    </v-list-item>

                    <v-list-item>
                      <v-list-item-icon>
                        <v-icon>mdi-account-group-outline</v-icon>
                      </v-list-item-icon>
                      <v-list-item-content>
                        <v-list-item-title>Users</v-list-item-title>
                      </v-list-item-content>
                    </v-list-item>

                  </v-list>
                </v-navigation-drawer>
              </v-card>

          </v-col>
        </v-row>
      </v-container>
    </v-content>
  </v-app>
</template>


<script>
export default {
  name: "App",

  data: () => ({
    //
  })
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