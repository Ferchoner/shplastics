<script setup lang="ts">

</script>

<template>
  <div class="float-elements position-relative">
    <div class="whatsapp-icon position-fixed">
      <a href="https://wa.link/04hcux" target="_blank" class="text-decoration-none m-0 p-0">
        <img src="~assets/images/icon-whatsapp_SHP.svg" alt="Contáctanos" class="img-fluid">
      </a>
    </div>
    <div class="phone-icon position-fixed">
      <a href="tel:+524621748147" target="_blank" class="text-decoration-none m-0 p-0">
        <img src="~assets/images/icon-telefono_SHP.svg" alt="Llámanos" class="img-fluid">
      </a>
    </div>
  </div>
</template>

<style scoped lang="sass">
.float-elements
  background: red
  height: 0
  width: 0
  z-index: 990
  @media (min-width: 675px)
  @media (min-width: 990px)
  @media (min-width: 1200px)
  @media (min-width: 1400px)

.phone-icon, .whatsapp-icon
  bottom: 25px
  right: 5px
  @media (min-width: 675px)
  @media (min-width: 990px)
  @media (min-width: 1200px)
    bottom: 35px
    right: 28px
  @media (min-width: 1400px)
    bottom: 35px
    right: 40px

  a
    position: relative
    img
      position: relative
      z-index: 990
      height: 50px
      width: 50px
      @media (min-width: 675px)
      @media (min-width: 990px)
      @media (min-width: 1200px)
        height: auto
        width: 100px
      @media (min-width: 1400px)
        height: auto
        width: 120px
.whatsapp-icon
  bottom: 80px
  @media (min-width: 675px)
  @media (min-width: 990px)
  @media (min-width: 1200px)
    bottom: 170px
  @media (min-width: 1400px)
    bottom: 200px

.phone-icon
  right: 15px
  @media (min-width: 675px)
  @media (min-width: 990px)
  @media (min-width: 1200px)
    right: 50px
  @media (min-width: 1400px)
    right: 65px
  a img
    height: 50px
    width: 50px
    @media (min-width: 675px)
    @media (min-width: 990px)
    @media (min-width: 1200px)
      height: auto
      width: 70px
    @media (min-width: 1400px)
      height: auto
      width: 90px
</style>