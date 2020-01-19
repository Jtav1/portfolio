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
    justintavaresContent: "<ul><li>",
    homelabContent: "heyay ya"
  })
};
</script>

<style></style>
