// 置き換わるくさい
<template>
  <v-app>
    <v-container fluid fill-height>
      <v-layout align-center justify-center>
        <v-flex xs12 sm8 md4>
          <v-card class="elevation-12">
            <v-toolbar dark color="primary">
              <v-toolbar-title>char num count</v-toolbar-title>
            </v-toolbar>
            <v-card-text>
              <p>{{ countCharNum }}</p>
              <v-text-field v-model="message" />
            </v-card-text>
          </v-card>
        </v-flex>
      </v-layout>
    </v-container>
  </v-app>
</template>

<script>
// コンポーネントわたすことになってんのか。
export default {
  data: function () {
    return {
      message: "Hello Vue!",
      cnt: "Hello Vue!".length,
    };
  },
  computed: {
    countCharNum: function () {
      return this.message.length;
    },
  },
};
</script>
