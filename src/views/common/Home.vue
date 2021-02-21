<template>

<v-container class="cards">
                <Card/>
                <Card2/>
</v-container>

</template>

<script>
import Card from './card/Card.vue'
import Card2 from './card/Card2.vue'
  export default {
    components: { 
        Card,
        Card2
        },
  }
</script>

<style scoped>

        .cards {
                display:flex;
                flex-direction: row;
        }

</style>

