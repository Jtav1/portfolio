<template>
  <v-app>
    <v-app-bar dense fixed>
      <v-app-bar-nav-icon></v-app-bar-nav-icon>

      <v-toolbar-title class="script">Justin Tavares's Homepage</v-toolbar-title>

      <v-spacer></v-spacer>
      <v-btn icon>
        <a href="resume.html"><v-icon>mdi-file-document</v-icon></a>
      </v-btn>
      <v-btn icon>
        <a href="https://www.linkedin.com/in/justin-tavares-b0459a5a/">
          <v-img src="./assets/icons8-linkedin-48.png"></v-img>
        </a>
      </v-btn>
      <v-btn icon>
        <a href="https://www.github.com/jtav1/">
          <v-img src="./assets/GitHub-Mark-32px.png"></v-img>
        </a>
      </v-btn>
      
    </v-app-bar>
    <v-main>
      <Homepage />
      <Portfolio />
      <Server />
      <LookingFor />
      <ContactMe />
    </v-main>
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
import Server from "./components/Server";
import LookingFor from "./components/LookingFor";
import ContactMe from "./components/ContactMe";

export default {
  name: "App",

  components: {
    Homepage,
    Portfolio,
    Server,
    LookingFor,
    ContactMe
  },

  data: () => ({
    //
  })
};
</script>
