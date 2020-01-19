<template>
  <div id="portfolio">
    <v-expansion-panels>
      <v-expansion-panel>
        <v-expansion-panel-header>
          <v-row>
            <v-col cols="12" sm="1" md="1" lg="1" xl="1">
              <v-img
                src="../assets/jtav.png"
                contain
                height="30"
                style="text-align:left;"
              ></v-img>
            </v-col>
            <v-col cols="12" sm="1" md="1" lg="1" xl="1">
              Justintavares.com
            </v-col>
          </v-row>
        </v-expansion-panel-header>
        <v-expansion-panel-content>
          <span v-html="justintavaresContent"></span>
        </v-expansion-panel-content>
      </v-expansion-panel>

      <v-expansion-panel>
        <v-expansion-panel-header>
          <v-row>
            <v-col cols="12" sm="1" md="1" lg="1" xl="1">
              <v-img
                src="../assets/server.png"
                contain
                height="30"
                style="text-align:left;"
              ></v-img>
            </v-col>
            <v-col cols="12" sm="1" md="1" lg="1" xl="1">
              Homelab
            </v-col>
          </v-row></v-expansion-panel-header
        >
        <v-expansion-panel-content>
          <span v-html="homelabContent"></span>
        </v-expansion-panel-content>
      </v-expansion-panel>
    </v-expansion-panels>
  </div>
</template>
<script>
export default {
  data: () => ({
    justintavaresContent: "<ul><li><a href='https://github.com/Jtav1/portfolio'>https://github.com/Jtav1/portfolio</a></li></ul>",
    homelabContent: "<p>Justin's homelab currently contains a Dell R710 running Unraid 6.8.1.</p><p>This server runs multiple docker containers as well as at least one linux VM at any given time</p><p>Future projects for this server may include a smart home server. Currently, the server runs a nextcloud instance, a reverse nginx proxy to enable SSL-enabled connections to websites hosted there, and webhosting for this site.</p>"
  })
};
</script>

<style></style>
