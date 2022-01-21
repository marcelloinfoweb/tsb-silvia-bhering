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

const url = 'https://wati-integration-service.clare.ai/ShopifyWidget/shopifyWidget.js?23726';
const s = document.createElement('script');
s.type = 'text/javascript';
s.async = true;
s.src = url;
const options = {
  "enabled": true,
  "chatButtonSetting": {
    "backgroundColor": "#4dc247",
    "ctaText": "",
    "borderRadius": "25",
    "marginLeft": "0",
    "marginBottom": "50",
    "marginRight": "50",
    "position": "right"
  },
  "brandSetting": {
    "brandName": "Sílvia Bhering",
    "brandSubTitle": "Terapeuta do Sono do Bebê",
    "brandImg": "https://cdn.clare.ai/wati/images/WATI_logo_square_2.png",
    "welcomeText": "Olá, Como posso ajudar?",
    "messageText": "Olá, Gostaria de mais informações",
    "backgroundColor": "#0a5f54",
    "ctaText": "Abrir o Whatsapp",
    "borderRadius": "25",
    "autoShow": false,
    "phoneNumber": "5531982486575"
  }
};
s.onload = function () {
  CreateWhatsappChatWidget(options);
};
var x = document.getElementsByTagName('script')[0];
x.parentNode.insertBefore(s, x);
</script>
<style>
.btn-whatsapp, .btn-whatsapp:hover {
  background: #25D366 !important;
  border-color: #25D366 !important;
  color: white !important;
}
</style>
