<template>
  <div id="homepage">
    
    <v-parallax src="../assets/pic.jpg">
      <v-layout column justify-center align-center>
        <v-flex xs12 sm8 md6>
          <div class="centerbanner">
            <h1 class="hirebanner">Justin Tavares</h1>
            <h2 class="hiresubbanner">Full Stack Developer</h2>
          </div>
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

<style scoped>
.hirebanner {
  font-size: 5em;
  -webkit-text-stroke-width: 1px;
  -webkit-text-stroke-color: black;
}

.hiresubbanner {
  font-size: 3em;
  -webkit-text-stroke-width: 1px;
  -webkit-text-stroke-color: black;
}

.centerbanner {
  text-align: center;
}

</style>
