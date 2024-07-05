<script setup lang="ts">

</script>

<template>
  <div class="container-fluid container-smart-world bg-main-color1 position-relative">
    <div id="smart-world-anchor" class="position-absolute"></div>
    <div class="row">
      <div class="container-fluid text-container">
        <div class="row">
          <div class="col text-cc text-center">
            <p class="text-metropolis text">
            <span class="text-metropolis-bold title">
              Smart World <br>
              Un aliado correcto de los canales de distribución</span>,
              nuestro trabajo coordinado nos permite ofrecer confianza,
              calidad y servicio
            </p>
          </div>
        </div>
        <div class="row">
          <div class="col image-cc text-center">
            <img src="~assets/images/icon-process1_SHP.svg" alt="Smart world 1" class="img-fluid smart-world-img-1"><br class="d-md-none">
            <img src="~assets/images/icon-process2_SHP.svg" alt="Smart world 2" class="img-fluid smart-world-img-2"><br class="d-md-none">
            <img src="~assets/images/icon-process3_SHP.svg" alt="smart world 3" class="img-fluid smart-world-img-3">
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped lang="sass">
#smart-world-anchor
  margin-top: -130px

.container-smart-world
  padding: 25px 0
  @media (min-width: 675px)
  @media (min-width: 990px)
  @media (min-width: 1200px)
  @media (min-width: 1400px)
    padding: 130px 0 130px
  .text-container
    max-width: 95%
    @media (min-width: 675px)
      max-width: 600px
    @media (min-width: 990px)
      max-width: 800px
    @media (min-width: 1200px)
      max-width: 1600px
    @media (min-width: 1400px)
      max-width: 1800px
    .text-cc
      padding: 20px 25px 20px
      color: #ffffff
      font-size: 15px
      @media (min-width: 675px)
        padding: 0 135px 0
        font-size: 22px
        line-height: 30px
      @media (min-width: 990px)
      @media (min-width: 1200px)
        font-size: 35px
        line-height: 40px
      @media (min-width: 1400px)
        font-size: 45px
        line-height: 50px
    .image-cc
      img
        width: 180px
        @media (min-width: 675px)
        @media (min-width: 990px)
        @media (min-width: 1200px)
        @media (min-width: 1400px)
          width: 260px

</style>