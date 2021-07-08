<template>
  <div id="skill">
    <v-container fluid>
      <v-card width="100vw">
        <v-card-title class="pa-5 justify-center display-1 font-italic">
          <v-icon style="font-size:33px">mdi-tools</v-icon>Skill
        </v-card-title>
        <v-row>
          <v-col cols="12" sm="6" md="6" class="pa-10">
            <v-row justify="center" align-content="center">
              <v-icon class="mt-1" style="font-size:33px">mdi-laptop</v-icon
              ><span class="mt-1 ml-1" style="font-weight:bold; font-size:24px"
                >Frontend</span
              >
            </v-row>
            <v-row justify="center" align-content="center">
              <span class="mt-2 mb-2 ml-1">主にFrontendを担当しており、Vue.jsで開発しております。</span>
            </v-row>
            <v-data-table
              :headers="headers"
              :items="frontend"
              :items-per-page="5"
              class="elevation-1 mt-4"
              hide-default-footer
            ></v-data-table>
          </v-col>
          <v-col cols="12" sm="6" md="6" class="pa-10">
            <v-row justify="center" align-content="center">
              <v-icon class="mt-1" style="font-size:33px">mdi-laptop</v-icon
              ><span class="mt-1 ml-1" style="font-weight:bold; font-size:24px"
                >Backend</span
              >
            </v-row>
            <v-row justify="center" align-content="center">
              <span class="mt-2 mb-2 ml-1">API開発はNode.jsを使っております。</span>
            </v-row>
            <v-data-table
              :headers="headers"
              :items="backend"
              :items-per-page="5"
              class="elevation-1 mt-4"
              hide-default-footer
            ></v-data-table>
          </v-col>
        </v-row>
        <v-row>
          <v-col cols="12" sm="6" md="6" class="pa-10">
            <v-row justify="center" align-content="center">
              <v-icon class="mt-1" style="font-size:33px">mdi-database</v-icon
              ><span class="mt-1 ml-1" style="font-weight:bold; font-size:24px"
                >DB</span
              >
            </v-row>
            <v-row justify="center" align-content="center">
              <span class="mt-2 mb-2 ml-1">業務でPostgreSQLを使っています。</span>
            </v-row>
            <v-data-table
              :headers="headers"
              :items="db"
              :items-per-page="5"
              class="elevation-1 mt-4"
              hide-default-footer
            ></v-data-table>
          </v-col>
          <v-col cols="12" sm="6" md="6" class="pa-10">
            <v-row justify="center" align-content="center">
              <v-icon class="mt-1" style="font-size:33px">mdi-server</v-icon
              ><span class="mt-1 ml-1" style="font-weight:bold; font-size:24px"
                >インフラ・サーバー</span
              >
            </v-row>
            <v-row justify="center" align-content="center">
              <span class="mt-2 mb-2 ml-1">業務でDockerを使っています。AWSは勉強中です。</span>
            </v-row>
            <v-data-table
              :headers="headers"
              :items="server"
              :items-per-page="5"
              class="elevation-1 mt-4"
              hide-default-footer
            ></v-data-table>
          </v-col>
        </v-row>
        <v-row>
          <v-col cols="12" sm="6" md="6" class="pa-10">
            <v-row justify="center" align-content="center">
              <v-icon class="mt-1" style="font-size:33px">mdi-toolbox</v-icon
              ><span class="mt-1 ml-1" style="font-weight:bold; font-size:24px"
                >その他</span
              >
            </v-row>
            <v-row justify="center" align-content="center">
              <span class="mt-2 mb-2 ml-1">
              その他、開発で使っているツールや、学生時代に使っていた言語です。
              </span>
            </v-row>
            <v-data-table
              :headers="headers"
              :items="other"
              :items-per-page="5"
              class="elevation-1 mt-4"
              hide-default-footer
            ></v-data-table>
          </v-col>
          <v-col cols="12" sm="6" md="6" class="pa-10">
            <v-row justify="center" align-content="center">
              <v-icon class="mt-1" style="font-size:33px"
                >mdi-format-list-bulleted</v-icon
              ><span class="mt-1 ml-1" style="font-weight:bold; font-size:24px"
                >保有資格</span
              >
            </v-row>
            <v-row justify="center" align-content="center">
              <span class="mt-2 mb-2 ml-1">資格保有数が少ないので、これから沢山取得できるようにします。</span>
            </v-row>
            <v-data-table
              :headers="headersQualification"
              :items="qualification"
              :items-per-page="5"
              class="elevation-1 mt-4"
              hide-default-footer
            ></v-data-table>
          </v-col>
        </v-row>
      </v-card>
    </v-container>
  </div>
</template>
<script>
export default {
  data() {
    return {
      headers: [
        {
          text: "技術",
          value: "tech"
        },
        { text: "経験年数", value: "year" },
        { text: "スキル", value: "skill" }
      ],
      frontend: [
        {
          tech: "JavaScript",
          year: "2年",
          skill: "☆☆☆"
        },
        {
          tech: "TypeScript",
          year: "1年",
          skill: "☆☆"
        },
        {
          tech: "HTML5",
          year: "2年",
          skill: "☆☆☆"
        },
        {
          tech: "CSS",
          year: "2年",
          skill: "☆☆"
        },
        {
          tech: "Vue.js",
          year: "2年",
          skill: "☆☆☆"
        },
        {
          tech: "React",
          year: "1年未満",
          skill: "☆"
        }
      ],
      backend: [
        {
          tech: "JavaScript",
          year: "2年",
          skill: "☆☆☆"
        },
        {
          tech: "TypeScript",
          year: "1年",
          skill: "☆☆"
        },
        {
          tech: "Node.js",
          year: "2年",
          skill: "☆☆"
        }
      ],
      db: [
        {
          tech: "PostgreSQL",
          year: "2年",
          skill: "☆☆"
        },
        {
          tech: "MySQL",
          year: "1年未満",
          skill: "☆☆"
        }
      ],
      server: [
        {
          tech: "AWS(EC2)",
          year: "1年未満",
          skill: "☆"
        },
        {
          tech: "Docker",
          year: "1年",
          skill: "☆"
        }
      ],
      other: [
        {
          tech: "Python",
          year: "4年",
          skill: "☆☆"
        },
        {
          tech: "C#",
          year: "2年",
          skill: "☆☆"
        },
        {
          tech: "gitLab",
          year: "2年",
          skill: "☆☆☆"
        },
        {
          tech: "slack",
          year: "4年",
          skill: "☆☆☆"
        }
      ],
      qualification: [
        {
          qualification: "JDLA G検定"
        },
        {
          qualification: "ビジネスキャリア検定"
        }
      ],
      headersQualification: [
        {
          text: "資格",
          value: "qualification"
        }
      ]
    };
  }
};
</script>
<style>
.v-data-table-header {
  color: #fff;
  background: #41a2e6;
}
</style>
