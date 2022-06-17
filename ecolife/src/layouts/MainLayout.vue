<template>
  <q-layout view="hhh lpR fff">
    <q-header style="background: transparent" reveal class="h-70px content-center">
      <q-toolbar>
        <div class="w-15pr h-50px mt-10px">
          <img
            src="http://demo.posthemes.com/pos_ecolife/layout2/img/ecolife-responsive-prestashop-theme-logo-1580528177.jpg"
            alt="" />
        </div>
        <div class="row w-85pr h-50px mt-10px content-center">
          <span class="span q-ml-xl text-subtitle2 text-weight-bold text-black">Home</span>
          <span class="span q-ml-xl text-subtitle2 text-weight-bold text-black">Fresh Food</span>
          <span class="span q-ml-xl text-subtitle2 text-weight-bold text-black">Fresh Vegetable</span>
          <span class="span q-ml-xl text-subtitle2 text-weight-bold text-black">Prices Drop</span>
          <span class="span q-ml-xl text-subtitle2 text-weight-bold text-black">Contact us</span>
          <q-space />
          <q-icon color="black" size="25px" name="search" class="q-mr-md" />
          <q-icon color="black" size="25px" name="lock" /><strong
            class="mt-3px mr-10px text-black text-weight-bold">$0.00</strong>
        </div>
      </q-toolbar>
    </q-header>

    <q-page-container>
      <router-view />
    </q-page-container>

    <q-footer bordered class="bg-black text-white q-mt-xl h-600px">
      <div class="w-100pr h-70pr row justify-center items-center content-center">
        <div class="w-92pr h-60pr row">
          <div class="w-25pr h-100pr">
            <div class="text-h6 text-weight-bolder text-white">
              OPENING HOURS
            </div>
            <div class="q-mt-lg text-grey text-weight-bold">
              Monday – Friday: 8am – 4pm
            </div>
            <div class="mt-10px text-grey text-weight-bold">
              Saturday: 9am – 5pm
            </div>
            <div class="q-mt-lg">
              <q-icon class="icon" name="fab fa-facebook-f" />
              <q-icon class="icon q-ml-md" name="fab fa-twitter" />
              <q-icon class="icon q-ml-md" name="fab fa-youtube" />
              <q-icon class="icon q-ml-md" name="fab fa-google" />
              <q-icon class="icon q-ml-md" name="fab fa-instagram-square" />
            </div>
          </div>
          <div class="w-25pr h-100pr">
            <div class="text-h6 text-weight-bolder text-white">INFORMATION</div>
            <div class="a-href column q-mt-lg text-weight-bold">
              <a href="">Dlivery</a>
              <a href="">About Us</a>
              <a href="">Secure Paymett</a>
              <a href="">Contact Us</a>
              <a href="">Sitemap</a>
            </div>
          </div>
          <div class="w-25pr h-100pr">
            <div class="text-h6 text-weight-bolder text-white">
              CUSTOM LINKS
            </div>
            <div class="a-href column q-mt-lg text-weight-bold">
              <a href="">Legal Notice</a>
              <a href="">Prices Drop</a>
              <a href="">New Product</a>
              <a href="">Best Sales</a>
              <a href="">Login</a>
            </div>
          </div>
          <div class="w-25pr h-100pr">
            <div class="text-h6 text-weight-bolder text-white">NEWSLETTER</div>
            <div class="q-mt-lg text-grey text-weight-bold">
              Be the first to know about our new arrivals and exclusive offers.
            </div>
            <div class="q-mt-md">
              <form>
                <q-input outlined type="email" bg-color="white" v-model="email" :dense="dense" />
              </form>
            </div>
          </div>
        </div>
      </div>
      <div class="row justify-center">
        <q-separator class="w-90pr bg-dark"> </q-separator>
      </div>
      <div class="w-100pr h-29pr column justify-center items-center content-center">
        <div>
          <img src="http://demo.posthemes.com/pos_ecolife_fastfood/img/cms/payment.png" alt="" />
        </div>
        <div class="q-mt-xl">Copyright © Posthemes. All Rights Reserved</div>
      </div>
    </q-footer>
  </q-layout>
</template>

<script>
import { ref } from "vue";

export default {
  setup() {
    return {
      email: ref(""),
      dense: ref(true),
    };
  },
};
</script>

<style>
.span {
  cursor: pointer;
  background: transparent;
}

.icon {
  color: grey;
}

.icon:hover {
  color: red;
  cursor: pointer;
}

.a-href a {
  text-decoration: none;
  color: grey;
}

.a-href a:hover {
  color: red;
  margin-left: 5px;
  cursor: pointer;
}

.a-href {
  line-height: 2.5;
  color: grey;
}
</style>
