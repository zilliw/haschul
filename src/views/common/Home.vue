<template>
    <div>
         <router-view></router-view>
         <component :is="HomeComponent" />
         <Home-menu-item> </Home-menu-item>
    </div>

</template>

<script>
    import HomeMenu from './HomeMenu.vue'
    import HomeMenuItem from './HomeMenuItem.vue'

    export default {
    name:'Home',

    components: {
        HomeMenu,
        HomeMenuItem
    },

    computed: {
      HomeComponent () {
        return this.$route.name
      }
    },


  }
</script>

<style scoped>
    .themes {
      padding-left: 10px;
      padding-top: 10px;
      padding-right:10px;
    }
</style>
