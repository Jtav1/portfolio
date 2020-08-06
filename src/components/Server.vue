<template>
  <div id="portfolio" class="server">
      <a id="server"></a>
    <span style="text-align:center;">
      <h2>How does this website work?</h2>
    </span>
    <div class="leftHalf"></div>
    <div class="rightHalf">
      <v-card class="mx-auto" max-width="500" min-height="350" outlined>
        <v-list-item three-line>
          <v-list-item-content>
            <div class="overline mb-4">Justin's Homelab</div>
            <v-list-item-title class="headline mb-1">An old Dell R710</v-list-item-title>
            <div class="text--primary, cardText">Justin's homelab currently contains a Dell R710 running Unraid 6.8.1</div>
            <div class="text--primary, cardText">This server runs multiple docker containers and linux VMs, and one Linux Mint workstation</div>
            <div class="text--primary, cardText">Future projects for this server may include a smart home server. Currently, the server runs a nextcloud instance, a reverse nginx proxy to enable SSL-enabled connections to websites hosted there, and webhosting for this site.</div>
            <div class="text--primary, cardText">This website runs in a docker container on an Ubuntu VM behind a reverse proxy that provides an SSL certificate</div>
          </v-list-item-content>
        </v-list-item>
      </v-card>
    </div>
  </div>
</template>
<script>
export default {
  data: () => ({
    //
  }),
};
</script>

<style>
.server {
  background-color: lightgrey;
  padding: 0em 0 5em 0;
  height: 500px;
}

.leftHalf {
  background: url(https://i.imgur.com/G9O9Btl.jpg);
  width: 50%;
  position: absolute;
  left: 0px;
  height: 400px;
  background-repeat: no-repeat;
}

.rightHalf {
  width: 50%;
  position: absolute;
  right: 0px;
  height: 400px;
  background-repeat: no-repeat;

}

.cardText {
    padding-bottom:10px;
}
</style>