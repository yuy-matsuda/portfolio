<template>
  <div id="contact">
    <v-container fluid>
      <v-card width="100vw">
        <v-card-title class="justify-center display-1 font-italic">
          <v-icon style="font-size:33px">mdi-email</v-icon>
          Contact
        </v-card-title>
        <v-card-text>
          <v-row justify="center" align-content="center">
            <v-col cols="15" sm="6" md="6" align="center">
              ご連絡はTwitterのDMまでお願いします。
            </v-col>
          </v-row>
          <v-row justify="center" align-content="center">
            <v-col cols="15" sm="6" md="6" align="center">
              <v-btn text :href="link" target="_blank">
                <v-icon left color="#1DA1F2">mdi-twitter</v-icon>
                <span>Twitter</span>
              </v-btn>
            </v-col>
          </v-row>
        </v-card-text>
      </v-card>
    </v-container>
  </div>
</template>
<script>
export default {
  data: () => ({
    link: "https://twitter.com/dmatsu_nn"
  })
};
</script>
<style></style>
