<template>
  <div class="main-corusel w-100pr ">
    <q-carousel swipeable animated arrows v-model="slide" infinite :autoplay="false" style="height: auto;">
      <q-carousel-slide class="w-100pr" :name="1">
        <q-img class="w-100pr h-610px"
          src="http://demo.posthemes.com/pos_ecolife_fastfood/modules/posslideshows/images/sample-1.jpg">
          <div class="w-100pr h-100pr row items-center" style="background: none">
            <div class="w-26pr h-33pr q-ml-xl" style="background: none">
              <div class="text-black">COFFEE CREAM & CHOCOLATE</div>
              <div class="text-h4 mt-7px text-black text-weight-bold">
                Girella Motta Cacao Soft Sponge Cake
              </div>
              <div class="q-mt-lg">
                <q-btn class="btn" unelevated rounded color="secondary" label="SHOP NOW" />
              </div>
            </div>
          </div>
        </q-img>
      </q-carousel-slide>

      <q-carousel-slide :name="2">
        <q-img class="w-100pr h-610px"
          src="http://demo.posthemes.com/pos_ecolife_fastfood/modules/posslideshows/images/sample-2.jpg">
          <div class="w-100pr h-100pr row items-center" style="background: none">
            <div class="w-26pr h-33pr q-ml-xl" style="background: none">
              <div class="text-black">COFFEE CREAM & CHOCOLATE</div>
              <div class="text-h4 mt-7px text-black text-weight-bold">
                Girella Motta Cacao Soft Sponge Cake
              </div>
              <div class="q-mt-lg">
                <q-btn class="btn" unelevated rounded color="secondary" label="SHOP NOW" />
              </div>
            </div>
          </div>
        </q-img>
      </q-carousel-slide>
      <template v-slot:control>
        <q-carousel-control position="bottom-right" :offset="[18, 18]">
        </q-carousel-control>
      </template>
    </q-carousel>
  </div>
</template>

<script>
import { ref } from "vue";

export default {
  setup() {
    return {
      slide: ref(1),
      autoplay: ref(true),
    };
  },
};
</script>
<style scoped>
.btn {
  padding: 5px 20px;
  font-size: 10px;
}

.q-carousel__slide,
.q-carousel .q-carousel--padding {
  padding: 0px;
}

.main-corusel {
  position: absolute;
  top: 0px
}
</style>
