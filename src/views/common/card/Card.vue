<template>

  <v-card
    elevation="24"
    max-width="444"
    class="mx-auto"
  >
    <v-system-bar
    color="#42b883" 
    height="50"
    dark
    position="center"
    >TOP 10 DES ARTICLES</v-system-bar>

    <v-carousel
      :continuous="false"
      :cycle="true"
      :show-arrows="false"
      hide-delimiter-background
      delimiter-icon="mdi-circle"
      height="300"
    >
      <v-carousel-item
        v-for="(slide, i) in slides"
        :key="i"
      >
        <v-sheet
          :color="colors[i]"
          height="100%"
          tile
        >
          <v-row
            class="fill-height"
            align="center"
            justify="center"
          >
            <div class="display-3">
              {{ slide }} Slide
            </div>      
          </v-row>
        </v-sheet>
      </v-carousel-item>
    </v-carousel>
        <v-list >
      <v-list-item>
        <v-list-item-avatar>
          <v-img src="../../../../public/images/hab.jpg"></v-img> </v-list-item-avatar>
        <v-list-item-content>
          <v-list-item-title>Hachim Abdallah</v-list-item-title>
          <v-list-item-subtitle>Auteur</v-list-item-subtitle>
        </v-list-item-content>
        <v-list-item-action>
          <v-rating
                readonly="true"
                background-color="#41b29a"  
                color="#41b29a"
                small > 
          ></v-rating>
                      <span class="primary--text subtitle-2">64<v-btn icon small><v-icon>mdi-thumb-up</v-icon></v-btn></span>
        </v-list-item-action>
      </v-list-item>
    </v-list>
  </v-card>
</template>

<script>
  export default {
      name: "Card",
    data () {
      return {
        colors: [
          'green',
          'secondary',
          'yellow darken-4',
          'red lighten-2',
          'orange darken-1',
        ],
        cycle: true,
        slides: [
            {item: 'First', rating: 4},
            {item: 'Second', rating: 5},
            {item: 'Third', rating: 2},
            {item: 'Fourth', rating: 3},
            {item: 'Fifth', rating: 3},

        ],
      }
    },
  }
</script>