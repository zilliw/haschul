<template v-slot:TheMenu>
 <v-app-bar
      app
      color="#42b883"
      flat
      dark
    > 

    <v-img max-height="100%" max-width="150px" position="left" contain src="../../../public/images/vuejs-logo.png"></v-img>

          <v-spacer></v-spacer>
          
          <v-text-field
            label="Rechercher un auteur, un thème..."
            dense
            flat
            hide-details
            rounded
            solo-inverted
          ></v-text-field>
          <v-spacer></v-spacer>
  

        <v-btn color="transparent" elevation="0">
            <v-icon > mdi-bell

            </v-icon>
        </v-btn>

        <v-btn color="transparent" elevation="0">
            <v-icon > mdi-mail

            </v-icon>
        </v-btn>

        <v-avatar label="avatar">
             <img
                src="../../../public/images/hab.jpg"
                alt="avatar"
            >
         </v-avatar>
    </v-app-bar>

</template>

<style scoped>

    .avatar {
        padding-right: 10px;
        padding-left: 10px;
    }

</style>
