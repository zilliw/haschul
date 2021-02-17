<template v-slot:TheMenu>
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
        <v-avatar>
             <img
                src="../../../public/images/hab.jpg"
                alt="avatar"
            >
         </v-avatar>

        <v-responsive max-width="260" class="avatar">
          
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

<style scoped>

    .avatar {
        padding-right: 10px;
        padding-left: 10px;
    }

</style>