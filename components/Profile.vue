<template>
    <div id="profile">
        <v-container
        fluid>
            <v-card
            width="100vw"
            >
            <v-card-title
            class="pa-5 justify-center display-1 font-italic"
            >
            <v-icon style="font-size:33px">mdi-account</v-icon>Profile
            </v-card-title>

            <v-row
            justify="center"
            align-content="center"
            >
                <v-col
                  cols="12"
                  sm="5"
                  md="5"
                  align="center"
                >
                <v-row
                justify="space-around"
                align-content="center"
                style="height:100%"
                >                
                <v-avatar
                width="80%"
                height="auto"
                >
                <img
                  src="qoo.jpg"
                  alt="SHOOT"
                  style="object-fit: cover;"
                >
                </v-avatar>
                </v-row>
                </v-col>
                <v-col
                  cols="12"
                  sm="6"
                  md="6"
                >
                <div style="font-size:20px">
                    はじめまして、Dmatsuと申します。平成5年生まれで社会人歴4年になりました。<br>
                    新卒で大手企業のSIerに入社し、1年目はWindowsアプリの開発しておりました。<br>
                    2年目からは、Webアプリ開発プロジェクトに参画し、主にFrontendの開発を現在しております。<br>
                    これからの展望としては、設計から開発だけでなく、マネジメントも学べればと思います。<br>
                    週に3回、同期ともくもく会を開催しており、興味をある分野を勉強中です。
                </div>
                </v-col>
            </v-row>
            </v-card>
        </v-container>
    </div>
</template>
<script>
  export default {
    data: () => ({
    }),
  }
</script>
<style>
</style>