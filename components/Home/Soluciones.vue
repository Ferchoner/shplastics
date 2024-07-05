<script setup lang="ts">

</script>

<template>
  <div class="container-fluid container-soluciones bg-main-color2 position-relative">
    <div id="soluciones-anchor" class="position-absolute"></div>
    <div class="row">
      <div class="container-fluid text-container">
        <div class="row">
          <div class="col text-cc text-center">
            <p class="text-metropolis text">
            <span class="text-metropolis-bold title">
              Gracias a nuestras soluciones
            </span>
              hemos logrado ayudar a la industria agrícola y alimentaria.
            </p>
          </div>
        </div>
        <div class="row">
          <div class="col-12 col-md  image-cc text-center main-color1 text-metropolis-bold">
            Productos para la<br>agricultura <br>
            <img src="~assets/images/p1_SHP.png" alt="Productos" class="img-fluid smart-world-img-3">
          </div>
          <div class="col-12 col-md image-cc text-center main-color1 text-metropolis-bold">
            Fabricación de<br>empaques <br>
            <img src="~assets/images/p2_SHP.png" alt="Productos" class="img-fluid smart-world-img-3">
          </div>
          <div class="col-12 col-md image-cc text-center main-color1 text-metropolis-bold">
            Soluciones para la<br>industria alimentaria <br>
            <img src="~assets/images/p3_SHP.png" alt="Productos" class="img-fluid smart-world-img-3">
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped lang="sass">
#soluciones-anchor
  margin-top: -100px

.container-soluciones
  padding: 25px 20px
  @media (min-width: 675px)
    padding: 130px 0 130px
  @media (min-width: 990px)
  @media (min-width: 1200px)
  @media (min-width: 1400px)

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
      padding: 20px 15px 0
      color: #ffffff
      font-size: 18px
      line-height: 25px
      @media (min-width: 675px)
        padding: 0 90px 0
        font-size: 35px
        line-height: 40px
      @media (min-width: 990px)
        font-size: 40px
        line-height: 45px
      @media (min-width: 1200px)
        padding: 0 135px 0
        font-size: 48px
        line-height: 55px
      @media (min-width: 1400px)

    .image-cc
      background-blend-mode: multiply
      background-color: #EDEDED88
      border-radius: 15px
      margin: 15px 0 0
      font-size: 20px
      line-height: 28px
      padding: 0 15px 0
      @media (min-width: 675px)
        border-radius: 25px
        margin: 100px 25px 0
        font-size: 25px
        line-height: 33px
        padding: 40px 35px 25px
      @media (min-width: 990px)
      @media (min-width: 1200px)
        font-size: 35px
        line-height: 40px
      @media (min-width: 1400px)
        font-size: 40px
        line-height: 50px
      img
        width: 180px
        margin: 30px 0 0
        @media (min-width: 675px)
        @media (min-width: 990px)
        @media (min-width: 1200px)
        @media (min-width: 1400px)
          margin: 30px 0 0
          width: 260px

</style>