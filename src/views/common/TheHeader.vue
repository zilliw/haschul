<template>
  <v-container mb-15>
    <v-app-bar
    app    
    color="#42b883"
    flat
    dark>
    
        <v-img max-height="100%" max-width="125px" position="left" contain src="../../../public/images/vuejs-logo.png"></v-img>
        <v-app-bar-nav-icon @click="drawer = !drawer"></v-app-bar-nav-icon>


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

        <v-btn icon><v-icon > mdi-bell </v-icon> </v-btn>
        <v-btn icon><v-icon > mdi-mail </v-icon> </v-btn>
        <v-btn icon >
                <v-avatar>
                        <img
                        src="../../../public/images/hab.jpg"
                        alt="avatar"
                        >   
                </v-avatar>
        </v-btn>
    </v-app-bar>

    <v-navigation-drawer
      v-model="drawer"
      fixed
      temporary
    >
        <TheMenu/>
    </v-navigation-drawer>
  </v-container>
</template>

<script>
import TheMenu from './TheMenu.vue'

  export default {
        components: { 
            TheMenu
        },

    data: () => ({ drawer: null }),
  }
</script>

<style scoped>

    .icon {
        padding-right: 15px;
        padding-left: 15px;
    }
    .p {
        font-size: 14px;
    }
</style>