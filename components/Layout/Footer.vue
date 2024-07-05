<script setup lang="ts">

</script>

<template>
  <div id="contacto-anchor" class="position-absolute"></div>
  <footer id="contacto" class="footer-container container-fluid bg-back-color m-0">
    <div class="row">
      <div class="col-12 col-md-6 container-logo px-0">
        <img src="~assets/images/logotipo_SHP.svg" alt="SH Plastics" class="img-fluid">
      </div>
      <div class="separador d-none d-md-block p-0">
      </div>
      <div class="col-12 col-md container-info">
        <a
            href="mailto:contacto@shplastics.com.mx"
            target="_blank"
            class="email-contact main-color1 text-decoration-none text-metropolis-bold"
        >
          contacto@shplastics.com.mx
        </a> <br>
        <a href="https://www.facebook.com/profile.php?id=100070130599769" target="_blank" class="fb-icon network-link text-decoration-none">
          <img src="~assets/images/icon-fb_SHP.svg" alt="Facebook" class="img-fluid facebook-icon">
        </a>
        <a href="https://www.instagram.com/shplastics" target="_blank" class="inst-icon network-link text-decoration-none">
          <img src="~assets/images/icon-instagram_SHP.svg" alt="Instagram" class="img-fluid instagram-icon">
        </a>
        <a href="https://www.linkedin.com/in/shplastics-smart-world-94aaba211/" target="_blank" class="li-icon network-link text-decoration-none">
          <img src="~assets/images/icon-linkedin_SHP.svg" alt="Linked In" class="img-fluid linkedin-icon">
        </a>
      </div>
      <div class="col-12 p-0 m-0"></div>
      <div class="col-12 text-end text-copyright">
        Copyright © {{ anio }} — SHPLASTICS <br>
        Todos los derechos reservados
      </div>
    </div>
  </footer>
</template>

<style scoped lang="sass">
footer.footer-container
  > div
    padding: 25px 20px 25px
    @media (min-width: 675px)
      padding: 150px 0 45px
    @media (min-width: 990px)
    @media (min-width: 1200px)
    @media (min-width: 1400px)


    .container-logo
      text-align: center
      img
        width: 100%
        max-width: 600px
        margin-bottom: 25px
        @media (min-width: 675px)
          max-width: 400px
          margin-top: 30px
          margin-bottom: 0
        @media (min-width: 990px)
        @media (min-width: 1200px)
        @media (min-width: 1400px)
          max-width: 600px

    .separador
      width: 0
      height: 150px
      border: 3px #dcdcdc solid
      border-radius: 5px
      @media (min-width: 675px)
      @media (min-width: 990px)
      @media (min-width: 1200px)
      @media (min-width: 1400px)

    .container-info
      text-align: center
      @media (min-width: 675px)
        text-align: right
        padding: 0 120px 0 0
      @media (min-width: 990px)
      @media (min-width: 1200px)
      @media (min-width: 1400px)

      a.email-contact
        font-size: 20px
        @media (min-width: 675px)
          font-size: 25px
        @media (min-width: 990px)
        @media (min-width: 1200px)
          font-size: 32px
        @media (min-width: 1400px)
          font-size: 55px

      a.network-link
        &.li-icon
          img
            margin-right: 0
        img
          width: 30px
          margin: 10px 10px 25px
          @media (min-width: 675px)
            width: 45px
            margin: 0 15px 70px
          @media (min-width: 990px)
          @media (min-width: 1200px)
          @media (min-width: 1400px)

    .text-copyright
      @media (min-width: 675px)
        padding: 0 120px 0 0
        font-size: 22px
        line-height: 35px
      @media (min-width: 990px)
      @media (min-width: 1200px)
      @media (min-width: 1400px)
</style>

<script>
export default {
  name: 'HomeFooter',
  data () {
    return {
      anio: new Date().getFullYear()
    }
  }
}
</script>