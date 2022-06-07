<template>
  <div class="q-pa-md h-730px">
    <q-carousel
      animated
      v-model="slide"
      navigation
      infinite
      :autoplay="autoplay"
      arrows
      transition-prev="slide-right"
      transition-next="slide-left"
      @mouseenter="autoplay = false"
      @mouseleave="autoplay = true"
      style="height: 700px;"
    >
      <q-carousel-slide :name="1" img-src="http://demo.posthemes.com/pos_ecolife/layout2/modules/posslideshows/images/03c53493b66e3228091fb5027e13aa8e78207328_1_2.jpg" />
      <q-carousel-slide :name="2" img-src="http://demo.posthemes.com/pos_ecolife/layout2/modules/posslideshows/images/081b9c1b802e10a8438349ca084ec5451f955c8e_2_2.jpg" />

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
