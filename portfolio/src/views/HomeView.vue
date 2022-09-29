<template >
  <v-app :style="{background: $vuetify.theme.themes.dark.background}">
    <Navbar />
  </v-app>
</template>

<script>
  import Navbar from "@/components/Navbar";

  export default { // eslint-disable-next-line
    name: 'Home',

    components: {
      Navbar,
    },
  }
</script>
