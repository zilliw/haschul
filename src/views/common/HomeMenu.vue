<template>
 <v-app-bar
      app
      color="#42b883"
      flat
      dark
    >        
    <v-btn
          v-for="link in links"
          :key="link"
          text
          center
        >
          {{ link }}
        </v-btn>

        <v-spacer></v-spacer>
        <v-avatar
          class="mr-10"
          color="grey darken-1"
          size="32"
        ></v-avatar>
        <v-responsive max-width="260">
          
          <v-text-field
            dense
            flat
            hide-details
            rounded
            solo-inverted
          ></v-text-field>
          
        </v-responsive>
        
    </v-app-bar>

</template>

<script>
  export default {
    data: () => ({
      links: [
        'Se connecter',
        'Concours du mois',
        'Articles',
        'Images',
      ],
    }),
  }
</script>