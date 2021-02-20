<template>
<div>
  <Card/>
    <Card2/>
  </div>
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