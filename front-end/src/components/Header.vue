<template>
  <v-app id="keep">
    <v-app-bar
      app
      clipped-left
      color="#7c56f6"
    >
      <v-icon
          class="mx-4"
          large
        >
          mdi-youtube
      </v-icon>
      <v-toolbar-title class="mr-12 align-center">
        <span class="title">Jaleko Acadêmicos</span>
      </v-toolbar-title>
    </v-app-bar>

     <v-footer
        app
        color="#7c56f6"
        class="white--text"
      >
        <span>Jaleko</span>
          <v-spacer>  <v-btn
                v-for="icon in icons"
                :key="icon"
                class="mx-4 white--text"
                icon
              >
                <v-icon size="24px">{{ icon }}</v-icon>
            </v-btn> </v-spacer>
        <span>&copy; {{ new Date().getFullYear() }}</span>
    </v-footer>          
  </v-app>
</template>

<script>
  export default {
    data: () => ({ 
      icons: [
        'mdi-facebook',
        'mdi-twitter',
        'mdi-linkedin',
        'mdi-instagram',
      ],

    }),
  }
</script>

<style>


</style>