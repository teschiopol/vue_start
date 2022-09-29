<template>
  <v-app-bar app color="#111111" dark flat class="px-8">
    <v-btn icon>
      <v-icon  color="#FFFFFF" @click="changeLogo()">fas fa-{{ iconName }}</v-icon>
    </v-btn>
    <v-spacer></v-spacer>
    <v-btn text @click="scroll('home')">Home</v-btn>
    <v-btn text @click="scroll('project')">Project</v-btn>
    <v-btn text @click="scroll('about')">About</v-btn>
    <v-btn text @click="scroll('contact')">Contact</v-btn>
  </v-app-bar>
</template>

<script>
export default { // eslint-disable-next-line
  name: "Navbar",
  data(){
    return {
      iconName: 'rocket'
    }
  },
  methods: {
    scroll(refName){
      const element = document.getElementById(refName);
      element.scrollIntoView({behavior:"smooth"});
    },
    changeLogo(){
      const iconName = this.iconName;
      switch (iconName) {
        case 'rocket':
          return this.iconName='dragon'
        case 'dragon':
            return this.iconName='bacon'
        case 'bacon':
            return this.iconName='bullseye'
        default:
          return this.iconName='rocket'
      }
    }
  }
}
</script>

<style scoped>

</style>
