<template>
  <div class="portfolio">
    <span style="text-align:center;">
      <h2>What am I looking for?</h2>
    </span>
    <v-carousel cycle interval="10000" height="400" hide-delimiter-background show-arrows-on-hover>
      <v-carousel-item v-for="(slide, i) in slides" :key="i">
        <v-sheet :color="colors[i]" height="100%">
          <v-row class="lookingForHeader" align="center" justify="center">
            <div class="display-1" style="padding-right: 10px;">
              {{ slide.title }}
            </div>
          </v-row>
          <v-row class="subtext" align="center" justify="center">
            <div class="subtext">
              {{ slide.subtext }}
            </div>
          </v-row>
        </v-sheet>
      </v-carousel-item>
    </v-carousel>
  </div>
</template>

<script>
export default {
  data() {
    return {
      colors: ["lightgrey", "lightgrey", "lightgrey", "lightgrey"],
      slides: [
        {
          title: "Remote-Friendly",
          subtext:
            "I am looking for a remote position with a North American company.",
        },
        {
          title: "Full Stack",
          subtext:
            "I have experience as a full stack developer working in a Javascript environment (Vue/Vuex, Nodejs/Express), and with dozens of other tech stacks (PHP, .NET, Java - see my Résumé for a full list).",
        },
        {
          title: "Front End",
          subtext:
            "I have experience building complicated front-end code using Javascript (Vue, React, Angular), component libraries (like Vuetify and Bootstrap) and various other technologies.",
        },
        {
          title: "Back End",
          subtext:
            "I have experience building complex back-ends and APIs for websites in various languages. I'm looking for a Javascript-based stack but I'm also comfortable in PHP and I am willing to learn other languages.",
        }
      ],
    };
  },
};
</script>
<style scoped>
.lookingForHeader {
    padding-top: 3em;
    
}
.subtext {
  padding: 3em 3em 3em 3em;
  max-width: 100%;
  text-align: center;
  justify-content: center;
}
</style>