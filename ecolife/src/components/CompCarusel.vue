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
      <q-carousel-slide :name="1" img-src="http://demo.posthemes.com/pos_ecolife/layout2/modules/posslideshows/images/03c53493b66e3228091fb5027e13aa8e78207328_1_2.jpg" />
      <q-carousel-slide :name="2" img-src="http://demo.posthemes.com/pos_ecolife/layout2/modules/posslideshows/images/081b9c1b802e10a8438349ca084ec5451f955c8e_2_2.jpg" />

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
