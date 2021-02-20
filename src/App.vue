<template>
        <v-app>

            <TheHeader/>
            <router-view/>
        
        </v-app>
</template>

<script>
import TheHeader from './views/common/TheHeader.vue'

export default {
    components: { 
        TheHeader
        }
  }
</script>

<style scoped>
    .app {
        font-family: 'Roboto', sans-serif !important;
        font-size: 14px;
    }

    .p {
                font-size: 14px;
    }
</style>>


