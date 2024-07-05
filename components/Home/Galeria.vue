<script setup lang="ts">

</script>

<template>
  <div class="container-fluid container-galeria position-relative">
    <div id="galeria-anchor" class="position-absolute"></div>
    <div class="row">
      <div class="col-12 text-center img-container d-inline">
        <img src="~assets/images/galeria/img01_SHP.png" alt="Galeria SH Plastics" class="img-fluid image-galery img-01">
        <img src="~assets/images/galeria/img02_SHP.png" alt="Galeria SH Plastics" class="img-fluid image-galery img-02">
        <img src="~assets/images/galeria/img03_SHP.png" alt="Galeria SH Plastics" class="img-fluid image-galery img-03">
        <div class="w-100"></div>
        <img src="~assets/images/galeria/img04_SHP.jpg" alt="Galeria SH Plastics" class="img-fluid image-galery img-04">
        <img src="~assets/images/galeria/img05_SHP.png" alt="Galeria SH Plastics" class="img-fluid image-galery img-05">
        <img src="~assets/images/galeria/img06_SHP.png" alt="Galeria SH Plastics" class="img-fluid image-galery img-06">
        <div class="w-100"></div>
        <img src="~assets/images/galeria/img07_SHP.png" alt="Galeria SH Plastics" class="img-fluid image-galery img-07">
        <img src="~assets/images/galeria/img08_SHP.png" alt="Galeria SH Plastics" class="img-fluid image-galery img-08">
        <img src="~assets/images/galeria/img09_SHP.png" alt="Galeria SH Plastics" class="img-fluid image-galery img-09">
      </div>
    </div>
  </div>
</template>

<style scoped lang="sass">
#galeria-anchor
  margin-top: -50px

.container-galeria
  padding: 30px 0
  @media (min-width: 675px)
  @media (min-width: 990px)
  @media (min-width: 1200px)
  @media (min-width: 1400px)
    padding: 70px 0
  .img-container
    .image-galery
      width: 110px
      margin: 2px 2px
      @media (min-width: 675px)
        width: 310px
      @media (min-width: 990px)
      @media (min-width: 1200px)
      @media (min-width: 1400px)
</style>