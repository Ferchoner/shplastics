<script setup lang="ts">

</script>

<template>
  <div id="nosotros-anchor" class="position-absolute"></div>
  <div class="container-fluid container-nosotros bg-back-color main-color2">
    <div class="row">
      <div class="col-12 col-md-7 mx-0 container-video desktop">
        <video v-if="!mobile" width="100%" autoplay @click="playVideo()">
          <source src="~assets/videos/spot-desktop_SHP.mp4" type="video/mp4">
          Your browser does not support HTML video
        </video>
        <video v-else width="100%" autoplay @click="playVideo()">
          <source src="~assets/videos/spot-mobil_SHP.mp4" type="video/mp4">
          Your browser does not support HTML video
        </video>
      </div>
      <div class="col">
        <div class="row">
          <div class="col nosotros-texto text-metropolis-bold px-md-0 pt-0">
            Somos una empresa mexicana que ofrece soluciones inteligentes al mercado
          </div>
        </div>
        <div class="row container-nosotros-lista">
          <div class="col nosotros-lista text-metropolis">
            <img class="img-fluid" src="~assets/images/bullets_SHP.svg" alt="bullet">Productos innovadores
            <br>
            <img class="img-fluid" src="~assets/images/bullets_SHP.svg" alt="bullet">Materiales reciclables
            <br>
            <img class="img-fluid" src="~assets/images/bullets_SHP.svg" alt="bullet">Productos de alta resistencia
          </div>
        </div>
      </div>
    </div>
  </div>
  <div class="container-fluid container-nosotros2">
    <div class="row">
      <div class="col-12 col-md-8 text-container">
        <p class="text-metropolis-bold title main-color1">
          Nacimos de la necesidad de atender la demanda de viveros.
        </p>
        <p class="text-metropolis text main-color2">
          Iniciamos operaciones en el año 2021 y actualmente brindamos soluciones al sector agrícola, así como a la industria alimentaría en México.
        </p>
      </div>
      <div class="col-12 col-md-4 images-container">
        <img src="~assets/images/icon-plantas_SHP.svg" alt="Smart World" class="img-fluid">
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Nosotros',
  data () {
    return {
      anio: new Date().getFullYear(),
      mobile: false
    }
  },
  methods: {
    updateSize() {
      let windowWidth = ref(window.innerWidth);
      this.mobile = windowWidth.value < 768;
    },
    playVideo() {
      let video = document.querySelector('.container-video video');
      if (video) {
        if (video.paused) {
          video.play()
        } else {
          video.pause()
        }
      }
    }
  },
  mounted() {
    let windowWidth = ref(window.innerWidth);
    this.mobile = windowWidth.value < 768;

    window.addEventListener("resize", this.updateSize);
  },
  unmounted() {
    window.removeEventListener("resize", this.updateSize);
  },
}
</script>

<style scoped lang="sass">
#nosotros-anchor
  margin-top: -20px
.container-nosotros
  font-size: 18px
  line-height: 25px
  border-radius: 25px
  max-width: 96%
  padding: 30px 30px
  @media (min-width: 675px)
    max-width: 600px
    font-size: 24px
    line-height: 36px
    padding: 50px 0
    border-radius: 50px
  @media (min-width: 990px)
    max-width: 800px
  @media (min-width: 1200px)
    max-width: 1600px
  @media (min-width: 1400px)
    font-size: 45px
    line-height: 52px
    max-width: 1800px
    padding-top: 125px
    padding-bottom: 125px

  .container-video
    padding: 0 0 30px
    @media (min-width: 675px)
      padding: 0 65px
    @media (min-width: 990px)
    @media (min-width: 1200px)
    @media (min-width: 1400px)

    video
      border-radius: 25px
      @media (min-width: 675px)
        border-radius: 50px
      @media (min-width: 990px)
      @media (min-width: 1200px)
      @media (min-width: 1400px)


  .nosotros-texto
    margin-top: -10px
    padding: 0 5px
    margin-bottom: 20px
    @media (min-width: 675px)
      margin-bottom: 50px
      margin-right: 65px
    @media (min-width: 990px)
    @media (min-width: 1200px)
    @media (min-width: 1400px)


  .nosotros-lista
    font-size: 15px
    line-height: 28px
    background-color: #ffffff
    border-radius: 15px
    padding: 10px 2px
    @media (min-width: 675px)
      background-color: #ffffff
      border-radius: 25px
      padding: 35px 5px
      margin-right: 65px
    @media (min-width: 990px)
      font-size: 20px
      line-height: 30px
    @media (min-width: 1200px)
      font-size: 25px
      line-height: 35px
    @media (min-width: 1400px)
      font-size: 30px
      line-height: 60px
    img
      width: 20px
      margin: 0 10px
      @media (min-width: 675px)
      @media (min-width: 990px)
      @media (min-width: 1200px)
      @media (min-width: 1400px)
        width: 40px
        margin: 0 30px
.container-nosotros2
  max-width: 95%
  padding: 30px 20px 30px
  @media (min-width: 675px)
    max-width: 600px
    padding: 55px 80px 55px
  @media (min-width: 990px)
    max-width: 800px
  @media (min-width: 1200px)
    max-width: 1600px
  @media (min-width: 1400px)
    max-width: 1800px

  .text-container
    font-size: 20px
    line-height: 28px
    @media (min-width: 675px)
    @media (min-width: 990px)
      font-size: 25px
      line-height: 35px
    @media (min-width: 1200px)
      font-size: 32px
      line-height: 40px
    @media (min-width: 1400px)
      font-size: 45px
      line-height: 55px

    .text
      margin-top: 30px
      font-size: 15px
      line-height: 20px
      @media (min-width: 675px)
      @media (min-width: 990px)
      @media (min-width: 1200px)
        font-size: 28px
        line-height: 35px
      @media (min-width: 1400px)
        font-size: 35px
        line-height: 55px
</style>