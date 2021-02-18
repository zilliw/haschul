<template class="container">
    <v-layout>
        <TheHeader/>
        <TheMenu/>
    </v-layout>
</template>

<script>
import TheMenu from './TheMenu.vue'
import TheHeader from './TheHeader.vue'

export default {
    name: 'Home',

    components: { 
        TheMenu,
        TheHeader
        }
  }
</script>

<style >
.container {
        display: flex;
        max-width: 100%;
        max-height: 100%;
}
.item {
        display: flex;
        height: 100%;
        }
</style>