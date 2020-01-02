<template>
  <v-app class="white">
    
    <v-app-bar
      fixed
      app
      class=""
      color="rgba(255,255,255,0.9)"
    >
      <v-toolbar-title v-text="title" class="title-text brown--text"/>
      <v-spacer />
    </v-app-bar>
    <v-content>
      <v-container fluid class="pa-0">
        <nuxt />
      </v-container>
    </v-content>
    <v-footer
      :fixed="fixed"
      app
    >
      <span>&copy; 2019</span>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  data () {
    return {
      title: 'Thomson Brewers'
    }
  }
}
</script>
<style>
  @import url('https://fonts.googleapis.com/css?family=Pacifico&display=swap');

  .title-text{
    font-family: 'Pacifico' , cursive;
    font-size: 2em;
  }

  .pacifico-font{
    font-family: 'Pacifico' , cursive;
  }

  @media only screen and (max-width: 600px) {
    
    .pacifico-font{
      font-family: 'Pacifico' , cursive;
      font-size: 1em;
    }

  }
</style>
