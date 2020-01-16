<template>
  <div id="homepage">
    <v-parallax src="../assets/pic.jpg">
      <v-layout column justify-center align-center>
        <v-flex xs12 sm8 md6>
          <v-card color="rgb(255, 255, 255, 0.8)">
            <v-card-title class="custom-selector headline">
              <h1 class="display-1 font-weight-thin mb-4">Justin Tavares</h1>
              <br />
            </v-card-title>
            <v-card-subtitle>
              <h3 class="text-center">
                <a href="resume.html">Résumé</a> ||
                <a href="https://www.linkedin.com/in/justin-tavares-b0459a5a/"
                  >Linkedin</a
                >
              </h3>
            </v-card-subtitle>
          </v-card>
        </v-flex>
      </v-layout>
    </v-parallax>
  </div>
</template>

<script>
export default {
  name: "homepage",

  data: () => ({})
};
</script>
