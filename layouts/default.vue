<script setup lang="ts">
</script>

<template>
  <div class="main-layout">
    <LayoutFloats />
    <LayoutHeader />
    <slot />
    <LayoutFooter />
  </div>
</template>

<style lang="sass">
.main-layout
  padding-top: 80px
  @media (min-width: 675px)
    padding-top: 150px
  @media (min-width: 990px)
  @media (min-width: 1200px)
  @media (min-width: 1400px)

</style>
