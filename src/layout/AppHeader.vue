<template>
  <header class="header-global">
    <base-nav class="navbar-main" transparent type="" effect="light" expand>
      <router-link slot="brand" class="navbar-brand mr-lg-5" to="/">
        <img src="img/brand/Logo-Silvia.png" alt="logo">
      </router-link>

      <div class="row" slot="content-header" slot-scope="{closeMenu}">
        <div class="col-6 collapse-brand">
          <a href="https://demos.creative-tim.com/vue-argon-design-system/documentation/">
            <img src="img/brand/Logo-Silvia.png">
          </a>
        </div>
        <div class="col-6 collapse-close">
          <close-button @click="closeMenu"></close-button>
        </div>
      </div>

      <ul class="navbar-nav align-items-lg-center ml-lg-auto">
        <li class="nav-item">
          <a class="nav-link nav-link-icon" href="https://www.facebook.com/tsbsilviabhering" target="_blank"
             rel="noopener"
             data-toggle="tooltip" title="Curta o Facebook">
            <i class="fa fa-facebook-square"></i>
            <span class="nav-link-inner--text d-lg-none">Facebook</span>
          </a>
        </li>
        <li class="nav-item">
          <a class="nav-link nav-link-icon" href="https://www.instagram.com/tsbsilviabhering/"
             target="_blank" rel="noopener" data-toggle="tooltip" title="Siga-me no Instagram">
            <i class="fa fa-instagram"></i>
            <span class="nav-link-inner--text d-lg-none">Instagram</span>
          </a>
        </li>
        <li class="nav-item">
          <a class="nav-link nav-link-icon" href="//bit.ly/tsbsilviabhering" target="_blank" rel="noopener"
             data-toggle="tooltip" title="Entre em contato no WhatsApp">
            <i class="fa fa-whatsapp"></i>
            <span class="nav-link-inner--text d-lg-none">WhatsApp</span>
          </a>
        </li>
      </ul>
    </base-nav>
  </header>
</template>
<script>
import BaseNav from "@/components/BaseNav";
import BaseDropdown from "@/components/BaseDropdown";
import CloseButton from "@/components/CloseButton";

export default {
  components: {
    BaseNav,
    CloseButton,
    BaseDropdown
  }
};
</script>
<style>
.navbar-brand img {
  height: 54px !important;
}

@media (max-width: 991.98px) {
  .navbar-collapse .collapse-brand img {
    height: 54px !important;
  }
}
</style>
