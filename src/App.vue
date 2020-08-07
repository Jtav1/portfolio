<template>
  <v-app>
    <v-app-bar dense fixed>

      <v-tooltip bottom>
        <template v-slot:activator="{ on, attrs }">
          <v-app-bar-nav-icon
          v-bind="attrs"
          v-on="on"
          ></v-app-bar-nav-icon>
          </template>
        <span>Projects - Coming Soon</span>
      </v-tooltip>


      <v-toolbar-title class="script">Justin's Homepage</v-toolbar-title>

      <v-spacer></v-spacer>
      <v-tooltip bottom>
        <template v-slot:activator="{ on, attrs }">
        <v-btn icon
          v-bind="attrs"
          v-on="on">
          <a href="resume.html"><v-icon>mdi-file-document</v-icon></a>
        </v-btn>
        </template>
        <span>Résumé</span>
      </v-tooltip>
       <v-tooltip bottom>
        <template v-slot:activator="{ on, attrs }">
        <v-btn icon
          v-bind="attrs"
          v-on="on">
        <a href="https://www.linkedin.com/in/justin-tavares-b0459a5a/">
          <v-img src="./assets/icons8-linkedin-48.png"></v-img>
        </a>
      </v-btn>
        </template>
        <span>Linkedin</span>
      </v-tooltip>
       <v-tooltip bottom>
        <template v-slot:activator="{ on, attrs }">
        <v-btn icon
          v-bind="attrs"
          v-on="on">
        <a href="https://www.github.com/jtav1/">
          <v-img src="./assets/GitHub-Mark-32px.png"></v-img>
        </a>
      </v-btn>
        </template>
        <span>Github</span>
      </v-tooltip>
      
      
      
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
