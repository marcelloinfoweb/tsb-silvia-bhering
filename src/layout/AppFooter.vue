<template>
  <footer class="footer has-cards">
    <div class="container">
      <div class="row row-grid align-items-center my-md">
        <div class="col-lg-6">
          <h3 class="text-primary font-weight-light mb-2">Obrigada pela visita!</h3>
          <h4 class="mb-0 font-weight-light">Pode entrar em contato em qualquer uma dessas plataformas.</h4>
        </div>
        <div class="col-lg-6 text-lg-center btn-wrapper">
          <a target="_blank" rel="noopener" href="https://www.facebook.com/tsbsilviabhering"
             class="btn btn-neutral btn-icon-only btn-facebook btn-round btn-lg" data-toggle="tooltip"
             data-original-title="Curta">
            <i class="fa fa-facebook-square"></i>
          </a>
          <a target="_blank" rel="noopener" href="https://www.instagram.com/tsbsilviabhering/"
             class="btn btn-neutral btn-icon-only btn-instagram btn-round btn-lg" data-toggle="tooltip"
             data-original-title="Curta">
            <i class="fa fa-instagram"></i>
          </a>
          <a target="_blank" rel="noopener" href="//bit.ly/tsbsilviabhering"
             class="btn btn-neutral btn-icon-only btn-whatsapp btn-round btn-lg" data-toggle="tooltip"
             data-original-title="Curta">
            <i class="fa fa-whatsapp"></i>
          </a>
        </div>
      </div>
      <hr>
      <div class="row align-items-center justify-content-md-between">
        <div class="col-md-6">
          <div class="copyright">
            &copy; {{ year }}
          </div>
        </div>
        <div class="col-md-6">
          <img src="//assets.pagseguro.com.br/ps-integration-assets/banners/seguranca/seguranca_468X60.gif"
               alt="Banner PagSeguro" title="Compre com PagSeguro e fique sossegado">
        </div>
      </div>
    </div>
  </footer>
</template>
<script>
export default {
  name: 'app-footer',
  data() {
    return {
      year: new Date().getFullYear()
    }
  }
};
</script>
<style>
.btn-whatsapp, .btn-whatsapp:hover {
  background: #25D366;
  border-color: #25D366;
  color: white;
}
</style>
