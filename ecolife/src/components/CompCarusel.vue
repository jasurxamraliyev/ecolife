<template>
  <div class="q-pa-md h-680px">
    <q-carousel
      swipeable
      animated
      arrows
      v-model="slide"
      infinite
      :autoplay="autoplay"
      style="height: 600px;"
    >
      <q-carousel-slide :name="1" >
        <q-img  src="http://demo.posthemes.com/pos_ecolife/layout2/modules/posslideshows/images/03c53493b66e3228091fb5027e13aa8e78207328_1_2.jpg" >
          <div  class="w-100pr h-100pr row items-center" style="background: none;">
            <div class="w-26pr h-33pr q-ml-xl" style="background: none;">
              <div class="text-black">
                  COFFEE CREAM & CHOCOLATE
              </div>
              <div class="text-h4 mt-7px text-black text-weight-bold">
                  Girella Motta Cacao
                   Soft Sponge Cake
              </div >
               <div class="q-mt-lg">
                 <q-btn class="btn" unelevated rounded color="secondary" label="SHOP NOW" />
               </div>
            </div>
          </div>
        </q-img>
      </q-carousel-slide>

      <q-carousel-slide :name="2">
        <q-img src="http://demo.posthemes.com/pos_ecolife/layout2/modules/posslideshows/images/081b9c1b802e10a8438349ca084ec5451f955c8e_2_2.jpg">
          <div  class="w-100pr h-100pr row items-center" style="background: none;">
            <div class="w-26pr h-33pr q-ml-xl " style="background: none;">
              <div class="text-black">
                 CACAO FRUTTI ROSSI
              </div>
              <div class="text-h4 mt-7px text-black text-weight-bold">
                  La Girella Motta
                  Diventa Rosa
              </div >
               <div class="q-mt-lg">
                 <q-btn class="btn" unelevated rounded color="secondary" label="SHOP NOW" />
               </div>
            </div>
          </div>
        </q-img>
      </q-carousel-slide>
      <template v-slot:control>
        <q-carousel-control
          position="bottom-right"
          :offset="[18, 18]"
        >

        </q-carousel-control>
      </template>
    </q-carousel>
  </div>
</template>

<script>
import { ref } from 'vue'

export default {
  setup () {
    return {
      slide: ref(1),
      autoplay: ref(true)
    }
  }
}
</script>
<style scoped>
.btn{
  padding: 5px 20px ;
  font-size: 10px;
}
</style>
