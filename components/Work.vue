<template>
  <div id="work">
    <v-container fluid>
      <v-card width="100vw">
        <v-card-title class="justify-center display-1 font-italic">
          <v-icon style="font-size:33px">mdi-format-list-bulleted</v-icon>
          Work
        </v-card-title>
        <v-row>
          <v-col
            v-for="(card, index) in cards"
            :key="card.index"
            :cols="card.flex.cols"
            :sm="card.flex.sm"
            :md="card.flex.md"
            class="pa-10"
          >
            <a :href="card.redirect_url">
              <v-hover v-slot:default="{ hover }">
                <v-card :elevation="hover ? 16 : 2">
                  <v-img
                    :src="card.src"
                    class="white--text align-end"
                    gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
                    height="200px"
                  >
                    <v-card-title v-text="card.title"></v-card-title>
                    <v-card-text v-text="card.skill"></v-card-text>
                  </v-img>
                </v-card>
              </v-hover>
            </a>
          </v-col>
        </v-row>
      </v-card>
    </v-container>
  </div>
</template>
<script>
export default {
  data: () => ({
    cards: [
      {
        title: "Portfolio Page",
        skill: "",
        src: "top.jpg",
        redirect_url: "http://localhost:3000/",
        flex: { cols: 12, sm: 6, md: 6 }
      }
    ]
  })
};
</script>
<style></style>
