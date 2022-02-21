<template>
  <v-app >
    <v-navigation-drawer
    app
    v-model="drawer"
    :clipped="$vuetify.breakpoint.mdAndUp"
    >
      <div>
       botones
      </div>
    </v-navigation-drawer>
    <v-app-bar app :clipped-left="$vuetify.breakpoint.lgAndUp">
      <v-app-bar-nav-icon @click="drawer = !drawer"></v-app-bar-nav-icon>
      <v-toolbar-title v-text="title"></v-toolbar-title>
    </v-app-bar>
    <v-main>
      <nuxt />
    </v-main>
  </v-app>
</template>

<script>
export default {
  name: "DefaultLayout",
  data() {
    return {
      drawer:false,
      title: "LEC COQ"
    };
  },
};
</script>
