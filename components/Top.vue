<template>
  <div id="top">
    <v-card width="100vw">
      <v-img
        class="white--text align-center text-center font-italic"
        :class="{
          headline: $vuetify.breakpoint.smAndDown,
          'display-1': $vuetify.breakpoint.mdAndUp
        }"
        src="top.jpg"
      >
        <p class="title">Dmatsu Portfolio</p>
        <p class="subTitle">System Enginner</p>
      </v-img>
    </v-card>
  </div>
</template>
<style scoped>
.v-application .title {
  font-size: 3.25rem !important;
  font-weight: bold;
  line-height: 3rem;
  letter-spacing: 0.0125em !important;
  font-family: "Roboto", sans-serif !important;
}
.v-application .subTitle {
  font-size: 3.25rem !important;
  font-weight: bold;
  line-height: 3rem;
  letter-spacing: 0.0125em !important;
  font-family: "Roboto", sans-serif !important;
}
</style>
