<template>
<v-list outlined  >
                <v-list-item
                  v-for="category in categories"
                  :key="category"
                  link

                >
                  <v-list-item-content >
                    <v-list-item-title>
                      {{ category }}
                    </v-list-item-title>
                  </v-list-item-content>
                </v-list-item>
                <v-divider> </v-divider>
                <v-list-item
                  v-for="theme in themes"
                  :key="theme"
                  link

                >
                  <v-list-item-content >
                    <v-list-item-title>
                      {{ theme }}
                    </v-list-item-title>
                  </v-list-item-content>
                </v-list-item>
              </v-list>
 
</template>

<script>
  export default {
    name: 'TheMenu',

    data: () => ({ 
      drawer: null,
      
      themes: [
        'La vérité de l\'être',
        'La dystopie',
        'Amour et luxure',
        'Les héros',
        'Le surnaturel',
        'La nostalgie',
        'La noirceur',
      ],
      categories: [
        'Créer un article',
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
      font-size: 20px;
    }
</style>