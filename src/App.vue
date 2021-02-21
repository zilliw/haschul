<template>
        <v-app>

            <TheHeader/>
            <router-view/>
            <TheFooter/>
        </v-app>
</template>

<script>
import TheHeader from './views/common/TheHeader.vue'
import TheFooter from './views/common/TheFooter.vue'

export default {
    components: { 
        TheHeader,
        TheFooter
        }
  }
</script>

<style scoped>
    .app {
        font-family: 'Roboto', sans-serif !important;
        font-size: 14px;
    }
</style>>


