<template>
  <v-footer dark padless>
    <v-card flat tile class="black white--text py-5 px-5 text-center" width="100%">
      <v-row>
        <v-col cols="12" sm="4">
          <v-card-text class="white--text pt-2">
            <v-btn icon>
              <v-icon color="#03a9f4">
                fas fa-rocket
              </v-icon>
            </v-btn>
          </v-card-text>
        </v-col>
        <v-col cols="12" sm="4">
          <v-card-text class="pt-2">
            <v-btn v-for="icon in icons" :key="icon" class="mx-1 white--text" icon>
              <v-icon size="24px">{{icon}}</v-icon>
            </v-btn>
          </v-card-text>
        </v-col>
        <v-col cols="12" sm="4">
          <v-card-text class="pt-2">
            <v-btn class="mx-1 white--text" icon>
              <v-icon color="#03a9f4">
                mdi-brain
              </v-icon>
              Elaborated by Pol
            </v-btn>
          </v-card-text>
        </v-col>
      </v-row>
    </v-card>
  </v-footer>
</template>

<script>
export default { // eslint-disable-next-line
  name: "Footer",
  data(){
    return{
      icons:["mdi-facebook", "mdi-linkedin", "mdi-twitter", "mdi-github"]
    }
  }
}
</script>

<style scoped>

</style>
