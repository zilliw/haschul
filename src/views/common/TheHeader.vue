<template>
    <v-app-bar
      app
      color="#42b883"
      flat
      dark
    >
        <v-img max-height="100%" max-width="125px" position="left" contain src="../../../public/images/vuejs-logo.png"></v-img>
                <v-spacer></v-spacer>
    <v-container class="py-0 fill-height">
              <v-responsive max-width="260">
          <v-text-field
            dense
            flat
            hide-details
            rounded
            solo-inverted
          ></v-text-field>
        </v-responsive>
                <v-spacer></v-spacer>
        <v-tab
          v-for="link in links"
          :key="link"
        >
          {{ link }}
        </v-tab>




      </v-container>
    </v-app-bar>
</template>


<script>
  export default {
    data: () => ({
      links: [
        'Market',
        'Activity',
        'Features',
        'Community',
        'Sign In',
      ],
    }),
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