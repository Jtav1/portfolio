<template>
  <v-app>
    <v-content>
      <Homepage />
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

export default {
  name: "App",

  components: {
    Homepage
  },

  data: () => ({
    //
  })
};
</script>
