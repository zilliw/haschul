<template class="container">
    <v-layout>
        <TheMenu>
        </TheMenu>
        <v-col>
                <v-row >
                        <TheThemeMenu>
                        </TheThemeMenu>
                </v-row>
        </v-col>
    </v-layout>
</template>

<script>
import TheThemeMenu from './TheThemeMenu.vue'
import TheMenu from './TheMenu.vue'

export default {
    name: 'Home',

    components: { 
        TheThemeMenu,
        TheMenu
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