<template>
  <v-app>
    <v-content>
      <Homepage />
      <span style="text-align:center;"><h2>Demo Reel</h2></span>
      <Portfolio />
    </v-content>
     <v-footer
        app
        absolute
        padless
				class="font-weight-medium"
			>
				<v-col
				class="text-center"
				cols="12"
				>
				{{ new Date().getFullYear() }} — <strong>Built with Vue/Vuetify</strong>
				</v-col>
			</v-footer>
  </v-app>
</template>

<script>
import Homepage from "./components/Homepage";
import Portfolio from "./components/Portfolio";

export default {
  name: "App",

  components: {
    Homepage,
    Portfolio
  },

  data: () => ({
    //
  })
};
</script>
