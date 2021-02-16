<template>
  <v-app id="inspire">
    <v-app-bar
      app
      color="#42b883"
      flat
      dark
      center
    >
        <v-img class="logo" max-height="100%" contain src="./../public/images/logo_bs_ocea.svg" color="white"></v-img>
                                      <v-spacer></v-spacer>
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

    <v-main class="grey lighten-3" >
        <v-row  class="themes">
          <v-col cols="2">
            <v-sheet>
              
              <v-list color="transparent">
                <v-list-item
                  v-for="theme in themes"
                  :key="theme"
                  link
                >
                  <v-list-item-content>
                    <v-list-item-title>
                      {{ theme }}
                    </v-list-item-title>
                  </v-list-item-content>
                </v-list-item>
              </v-list>
            </v-sheet>
          </v-col>

          <v-col>
              <v-row>
          <template v-for="category in categories">
            <v-col
              :key="category"
              class="mt-2"
              cols="12"
            >
              <strong> {{ category }}</strong>
            </v-col>

            <v-col
              v-for="j in 6"
              :key="`${category}${j}`"
              cols="6"
              md="2"
            >
              <v-sheet height="150"></v-sheet>
            </v-col>
          </template>
        </v-row>
          </v-col>
        </v-row>
    </v-main>
  </v-app>
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
      themes: [
        'La vérité de lêtre',
        'La dystopie',
        'Amour et luxure',
        'Les héros',
        'Le surnaturel',
        'La nostalgie',
        'La noirceur',
      ],
      categories: [
        'Top 10 des articles lus',
        'Articles recommandés',
      ]
    }),
  }
</script>

<style scoped>
    .themes {
      padding-left: 10px;
      padding-top: 10px;
      padding-right:10px;
    }
</style>