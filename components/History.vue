<template>
  <div id="history">
    <v-container fluid>
      <v-card width="100vw">
        <v-card-title class="pa-5 justify-center display-1 font-italic">
          <v-icon style="font-size:33px">mdi-timeline-outline</v-icon>History
        </v-card-title>
        <v-timeline :dense="$vuetify.breakpoint.smAndDown">
          <v-timeline-item color="purple lighten-2" fill-dot right>
            <v-card>
              <v-card-title class="purple lighten-2">
                <h2 class="text-h4 white--text font-weight-light">
                  千葉工業大学 [2012~2016]
                </h2>
              </v-card-title>
              <v-container>
                <v-row>
                  <v-col cols="12" md="10">
                    学部生時代は、ロボット工学を学んでいました。
                  </v-col>
                </v-row>
              </v-container>
            </v-card>
          </v-timeline-item>

          <v-timeline-item color="amber lighten-1" fill-dot left small>
            <v-card>
              <v-card-title class="amber lighten-1 justify-end">
                <h2 class="text-h4 mr-4 white--text font-weight-light">
                  千葉工業大学大学院 [2016~2018]
                </h2>
              </v-card-title>
              <v-container>
                <v-row>
                  <v-col cols="12" md="8">
                    機械学習に興味があったため、<br>院生時代はpythonを使ってDeepLearningの研究をやっていました。
                  </v-col>
                </v-row>
              </v-container>
            </v-card>
          </v-timeline-item>

          <v-timeline-item color="cyan lighten-1" fill-dot right>
            <v-card>
              <v-card-title class="cyan lighten-1">
                <h2 class="text-h4 white--text font-weight-light">
                  大手SIer入社 [2018~2021]
                </h2>
              </v-card-title>
              <v-container>
                <v-row>
                  <v-col cols="12" md="8">
                    <h3>1年目</h3>
                    C#でWindowsアプリを開発していました。<br>
                    最適化手法を使った波形解析アプリを開発していました。
                  </v-col>
                  <v-col cols="12" md="8">
                    <h3>2年目 - 4年目</h3>
                    Webアプリ開発チームに参画し、FrontendからBackendまで幅広く開発に携わりました。
                    現在は主にFrontend開発を行っています。
                  </v-col>
                </v-row>
              </v-container>
            </v-card>
          </v-timeline-item>
        </v-timeline>
      </v-card>
    </v-container>
  </div>
</template>
<script>
export default {
  data: () => ({
    items: [
      {
        color: "red lighten-2",
        icon: "mdi-star"
      },
      {
        color: "purple darken-1",
        icon: "mdi-book-variant"
      },
      {
        color: "green lighten-1",
        icon: "mdi-airballoon"
      },
      {
        color: "indigo",
        icon: "mdi-buffer"
      }
    ]
  })
};
</script>
<style></style>
