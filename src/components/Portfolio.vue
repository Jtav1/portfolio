<template>
  <div id="portfolio" class="portfolio">
    <span style="text-align:center;"><h2>What can Justin do for you?</h2></span>
        <v-container fluid>
      <v-row dense>
        <v-col
          v-for="card in cards"
          :key="card.title"
          :cols="card.flex"
        >
          <v-card>
            <v-img
              :src="card.src"
              class="white--text align-end"
              gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
              height="200px"
            >
              <v-card-title v-text="card.title"></v-card-title>
            </v-img>

            <v-card-actions>
              <v-spacer></v-spacer>
                <v-btn icon>
                <a :href="card.link">
                  <v-img src="../assets/GitHub-Mark-32px.png"></v-img>
                </a>
              </v-btn>
            </v-card-actions>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>
<script>
export default {
  data: () => ({
    cards: [
      { title: "Front End Stuff", src: "https://i.imgur.com/7Na2IkL.jpg", flex: 4, link: "https://github.com/Jtav1/portfolio", icon: "../assets/GitHub-Mark-32px.png" },
      { title: "Back End Stuff", src: "https://i.imgur.com/VxBnHZ4.png", flex: 4, link: "https://github.com/Jtav1/covid-19-project-backend", icon: "../assets/GitHub-Mark-32px.png" },
      { title: "Server Stuff", src: "https://upload.wikimedia.org/wikipedia/commons/thumb/0/09/Wikimedia_Foundation_Servers-8055_43.jpg/1280px-Wikimedia_Foundation_Servers-8055_43.jpg", flex: 4, link: "#server", icon:"mdi-server" },
    ]
 })
};
</script>

<style>
.portfolio {
  background-color: lightgrey;
  padding: 5em 0 5em 0;
}
</style>
