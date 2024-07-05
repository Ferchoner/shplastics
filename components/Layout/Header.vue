<script setup lang="ts">

</script>

<template>
  <div class="sh-header-container container-fluid px-md-5 position-fixed">
    <header class="sh-header d-none d-md-flex flex-wrap justify-content-start py-3 mb-4">
      <a href="/" class="sh-logo d-flex align-items-center mb-3 mb-md-0 text-dark text-decoration-none">
        <img class="img-fluid" src="~assets/images/logotipo_SHP.svg" alt="SH Plastics">
      </a>
      <ul class="nav">
        <li class="nav-item text-metropolis">
          <a href="/#nosotros-anchor" class="nav-link main-color1 active" aria-current="page">
            Nosotros
          </a>
        </li>
        <li class="nav-item text-metropolis">
          <a href="/#smart-world-anchor" class="nav-link main-color1">
            Smart World
          </a>
        </li>
        <li class="nav-item text-metropolis">
          <a href="/#soluciones-anchor" class="nav-link main-color1">
            Soluciones
          </a>
        </li>
        <li class="nav-item text-metropolis">
          <a href="/#galeria-anchor" class="nav-link main-color1">
            Galería
          </a>
        </li>
        <li class="nav-item text-metropolis">
          <a href="/#contacto-anchor" class="nav-link main-color1">
            Contacto
          </a>
        </li>
      </ul>
    </header>
    <header class="sh-header-mobile d-flex d-md-none flex-wrap justify-content-between py-3 mb-4">
      <a href="/" class="sh-logo d-flex align-items-center mb-3 mb-md-0 text-dark text-decoration-none">
        <img class="img-fluid" src="~assets/images/logotipo_SHP.svg" alt="SH Plastics">
      </a>
      <div class="hamburger-lines d-flex" @click="toggleMenu()">
        <span class="line line1"></span>
        <span class="line line2"></span>
        <span class="line line3"></span>
      </div>
    </header>
    <div class="header-menu-container position-fixed w-100 h-100 bg-back-color">
      <ul class="list-container text-metropolis-bold main-color1">
        <li class="menu-item nosotros">
          <a
            href="/#nosotros-anchor"
            class="link-menu-item text-metropolis-bold main-color1 nosotros"
            @click="toggleMenu()"
          >
            Nosotros
          </a>
        </li>
        <li class="menu-item Smart World">
          <a
            href="/#smart-world-anchor"
            class="link-menu-item text-metropolis-bold main-color1 smart-world"
            @click="toggleMenu()"
          >
            Smart World
          </a>
        </li>
        <li class="menu-item Soluciones">
          <a
            href="/#soluciones-anchor"
            class="link-menu-item text-metropolis-bold main-color1 soluciones"
            @click="toggleMenu()"
          >
            Soluciones
          </a>
        </li>
        <li class="menu-item Galería">
          <a
            href="/#galeria-anchor"
            class="link-menu-item text-metropolis-bold main-color1 galería"
            @click="toggleMenu()"
          >
            Galería
          </a>
        </li>
        <li class="menu-item Contacto">
          <a
            href="/#contacto-anchor"
            class="link-menu-item text-metropolis-bold main-color1 contacto"
            @click="toggleMenu()"
          >
            Contacto
          </a>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: 'LayoutHeader',
  data () {
    return { }
  },
  methods: {
    toggleMenu() {
      let toggler = document.querySelector('.hamburger-lines');
      if (toggler) {
        toggler.classList.toggle('open')
      }
      let menu = document.querySelector('.header-menu-container');
      if (menu) {
        menu.classList.toggle('open');
      }
    }
  }
}
</script>

<style scoped lang="sass">
.sh-header-container
  background: rgb(255,255,255)
  background: -moz-linear-gradient(0deg, rgba(255,255,255,0) 1%, rgba(255,255,255,0.31416316526610644) 25%, rgba(255,255,255,0.9556197478991597) 95%)
  background: -webkit-linear-gradient(0deg, rgba(255,255,255,0) 1%, rgba(255,255,255,0.31416316526610644) 25%, rgba(255,255,255,0.9556197478991597) 95%)
  background: linear-gradient(0deg, rgba(255,255,255,0) 1%, rgba(255,255,255,0.31416316526610644) 25%, rgba(255,255,255,0.9556197478991597) 95%)
  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr="#ffffff",endColorstr="#ffffff",GradientType=1)
  top: 0
  max-width: 100%
  width: 100vw
  z-index: 990
  .sh-header
    .nav-item
      font-size: 25px
      padding: 0 30px
      position: relative
      align-content: end

      @media (min-width: 675px)
      @media (min-width: 990px)
      @media (min-width: 1200px)
      @media (min-width: 1400px)
        font-size: 45px
        padding: 0 50px

      a
        padding: 0
        font-size: 18px
        @media (min-width: 675px)
          font-size: 20px
        @media (min-width: 990px)
        @media (min-width: 1200px)
        @media (min-width: 1400px)
          font-size: 28px

    .sh-logo
      padding: 0 30px 0
      img
        width:  60px
        @media (min-width: 990px)
          width:  100px
        @media (min-width: 1200px)
          width:  300px
        @media (min-width: 1400px)
          width:  400px

  .sh-header-mobile
    max-width: 100%
    .sh-logo
      padding: 0 0
      img
        width: 200px
    .hamburger-lines
      margin: 4px 10px 0 0
      height: 20px
      width: 25px
      z-index: 997
      flex-direction: column
      justify-content: space-between

      .line
        display: block
        height: 4px
        width: 100%
        border-radius: 10px
        background: #0e2431

      .line1
        transform-origin: 0 0
        transition: transform 0.4s ease-in-out

      .line2
        transition: transform 0.2s ease-in-out

      .line3
        transform-origin: 0 100%
        transition: transform 0.4s ease-in-out

      &.open
        .line1
          transform: rotate(45deg)

        .line2
          transform: scaleY(0)

        .line3
          transform: rotate(-45deg)
  .header-menu-container
    top: -100vh
    left: 0
    z-index: 995
    transition: top 800ms
    padding: 85px 0 0
    &.open
      top: 0
    ul
      margin: 0
      padding: 0
      text-align: center
      li
        list-style: none
        margin: 0 0 40px
        a
          text-decoration: none
          font-size: 30px

</style>