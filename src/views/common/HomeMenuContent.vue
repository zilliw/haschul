<template>
  <div>
    <v-layout class="content pt-0">
      <slot />
    </v-layout>
  </div>
</template>
<script>

export default {
  name: 'TheHomeSlot'
}
</script>

<style lang="scss" scoped>
    @import '../../../public/variables';
    .content {
      padding: 20px 25px;
      display: flex;
      justify-content: space-around;
    }
</style>
