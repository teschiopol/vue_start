<template >
  <v-app id="home" :style="{background: $vuetify.theme.themes.dark.background}">
    <Navbar />
    <v-container fluid>
      <v-row>
        <v-col cols="6">
          <v-img src="home_unicorn.png" contain max-height="500px"></v-img>
        </v-col>
        <v-col cols="6">
          <h4 class="white--text text-darken-4 top">Hi, I'm Pol!</h4>
          <h1 class="light-blue--text">Full Stack Developer</h1>
          <p class="grey--text">
            Whatever You dream, I'll do the impossible to code it!<br>
            Nice to meet You, this happy friend is Unicorne and our helper<br>
            during the journey that We are going to start...
          </p>
          <v-btn title color="light-blue" dark>About Me</v-btn>
        </v-col>
      </v-row>
    </v-container>
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
<style scoped>
  .top{
    margin-top: 180px;
  }
  .topInverse{
    margin-top: -250px;
  }
  .topTolbar{
    margin-top: 100px;
    text-align: center;
  }
  .first{
    width: 100%;
    height: 610px;
    background: linear-gradient(
      to right,
      #181818,
      #181818 50%,
      #111111 50%,
      #111111 50%
    );
    text-align: center;
    padding: 2rem 2rem;
  }
  .second{
    width: 100%;
    height: 400px;
    background: #181818;
    text-align: center;
    padding: 2rem 2rem;
  }
  .secondChild{
    display: inline-block;
    padding: 2rem 1rem;
    background-color: #1e1e1e;
    vertical-align: middle;
    text-align: left;
    margin-top: 250px;
  }
  .child{
    display: inline-block;
    padding: 2rem 1rem;
    margin-right: 8px;
    vertical-align: middle;
    text-align: left;
  }
  .bgcolor1{
    background-color: #1e1e1e;
  }
  .bgcolor2{
    background-color: #03a9f4;
  }
  .child1{
    display: inline-block;
    padding: 2rem 1rem;
    margin-right: 5px;
    vertical-align: middle;
    width: 240px;
  }
  .child2{
    display: inline-block;
    width: 245px;
    vertical-align: middle;
  }
  .mRight{
    margin-right: 8px;
  }
  .mButton{
    margin-bottom: 8px;
  }
  .padding{
    padding: 8px 0;
  }
  .col-12.pad{
    padding: 12px 0 !important;
  }
  .col-12.childcol{
    padding: 0 !important;
  }
  h1.number{
    font-size: 50px;
    font-weight: bold;
  }
</style>
