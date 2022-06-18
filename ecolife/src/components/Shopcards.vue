<template>
  <div>
    <nav class="bg-grey-2 w-100pr h-50px fit row no-wrap justify-center items-center content-center"> <span class="row mr-40pr">There are 16 products</span>
    <span class="mr-10pr">Sort by:</span><span><q-btn-dropdown color="white" class="text-black" label="Relevance" rounded></q-btn-dropdown></span></nav>
    <div class="fit row wrap justify-start items-start">
      <div v-for="i in 12" :key="i" class="w-235px h-450px q-mx-md border br-4px" style="margin-bottom:100px; margin-top:100px;">
        <div class="d-f jc-sp_btw q-mt-md">
          <div class="bg-red br-4px text-white text-weight-bold q-ml-md">-10%</div>
          <div class="bg-red br-4px text-white text-weight-bold w-50px  text-center q-mr-md">New</div>
        </div>
        <q-img class="img" src="http://demo.posthemes.com/pos_ecolife_fastfood/427-home_default/pizza-primavera.jpg"/>
  <div class="q-pa-md">
    <div class="q-gutter-y-md column">
      <q-rating
        v-model="ratingModel"
        size="24px"
        color="yellow-5"
        icon="star_border"
        icon-selected="star"
      />
    </div>
    <!-- button -->
  </div>
        <div class="text-h6 q-ml-md">Pizza Mushrooms</div>
        <div class="q-ml-md">Block out the haters with the fresh adidas® Originals Kaval <br></div> <br>
        <div class="text-italic q-ml-md d-f"><del class="fs-19px text-weight-light">$11.90</del><span class="text-red q-ml-md text-weight-bolder fs-20px">$10.12</span>
        </div>
        <!-- <div class="d-f">
          <div> <q-icon name="search"/><div class="text-p">Taqqoslang</div></div>
          <div> <q-icon name="search" class="q-ml-md"/><div class="text-p q-ml-md">Taqqoslang</div></div>
          <div class="text-center bg-red"> <q-icon class="q-ml-lg q-mt-md" name="fas fa-shopping-bag"/></div>
        </div> -->
      </div>
    </div>
  </div>
</template>

<script>
import { ref } from 'vue'

export default {
  setup () {
    return {
      ratingModel: ref(3),
      ratingModell: ref(1)
    }
  }
}
</script>
<style scoped>
.border{
  border: 1px solid rgb(214, 210, 210);
}
.border:hover{
  border: 1px solid rgb(223, 44, 44);

}
.position{
  position: absolute;
  top: 3460px;
  margin: 80px;

}
.but .position{
  opacity: 0;
}
.but .position:hover{
  opacity: 1;
}
</style>
