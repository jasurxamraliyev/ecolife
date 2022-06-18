<template>
  <q-page>

    <div class="w-100pr row  justify-between mt-2pr">
    <div class="w-30pr pl-7pr">
      <span class="text-h5">Filter By</span>
      <br>
      <q-separator color="red" class="w-16pr text-weight-bold ml-m100pr"></q-separator>
      <br>
      <!-- <div >
        <q-btn color="" text-color="white" label="x Clear" class="btn"/>
      </div> -->
      <span class="text-h6">categories</span>
      <div class="column">
        <q-checkbox v-model="right" label='Fudge Cookies(17)' class="chekbox"/>
        <q-checkbox v-model="right1" label='Rose Cookies(17)' class="chekbox"/>
        <q-checkbox v-model="right2" label='moravian spice(17)' class="chekbox"/>
        <q-checkbox v-model="right3" label='Sugar Cookies(17)' class="chekbox"/>
        <br>
        <span class="text-h6">Price</span>
        <br>
        <span>$9.00 - $34.00</span>
        <br>
        <div class="w-80pr" >
          <q-range color="red"/>
        </div>
        <div>
          <span class="text-h6">size</span>
          <br>
          <div class="column">
            <q-checkbox v-model="right4" label='S(4)' class="chekbox"/>
            <q-checkbox v-model="right5" label='M(4)' class="chekbox"/>
            <q-checkbox v-model="right6" label='L(4)' class="chekbox"/>
            <q-checkbox v-model="right7" label='XL(4)' class="chekbox"/>
          </div>
          <br>
          <div>
            <span class="text-h6">color</span>
            <br>
            <div class="column">
              <q-checkbox  label='grey(2)' color="grey" class="chekbox"/>
              <q-checkbox  label='white(5)' color="white" class="chekbox"/>
              <q-checkbox  label='black(5)' color="black" class="chekbox"/>
              <q-checkbox  label='camel(2)' color="brown" class="chekbox"/>
            </div>
            <br>
            <div>
              <span class="text-h6">Brand</span>
              <div class="column">
                <q-checkbox  v-model="right8" label='Studio Design(10)' color="grey" class="chekbox"/>
                <q-checkbox  v-model="right9" label='Graphik corner(7)' color="white" class="chekbox"/>
              </div>
              <br>
              <span class="text-h6">Dimansion</span>
              <div class="column">
                <q-checkbox  v-model="right8" label='40x60sm(5)' color="grey" class="chekbox"/>
                <q-checkbox  v-model="right9" label='60x90sm(5)' color="white" class="chekbox"/>
                <q-checkbox  v-model="right9" label='80x120sm(5)' color="white" class="chekbox"/>
              </div>
              <br>
              <div>
                <span class="text-h6">Tags</span>
                <q-separator color="red" class="w-16pr text-weight-bold ml-m100pr"></q-separator>
                <br>
                <div>
                  <q-btn class="btn" rounded label='cookies'/>
                  <q-btn class="btn" rounded label='cream cake'/>
                  <br><br>
                  <q-btn class="btn" rounded label='chocolate cake'/>
                  <q-btn class="btn" rounded label='Rose cookies'/>
                </div>

                <q-img src="http://demo.posthemes.com/pos_ecolife_fastfood/modules/ps_advertising/img/advertising-s1.jpg" width="80%" class="for_hover mt-80px"></q-img>

              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="w-70pr">
      <Shopcards/>
    </div>
    </div>

  </q-page>
</template>
<script>

import { ref } from 'vue'
import Shopcards from 'src/components/Shopcards.vue'

export default {
    setup() {
        return {
            left: ref(true),
            right: ref(false),
            left1: ref(true),
            right1: ref(false),
            left2: ref(true),
            right2: ref(false),
            left3: ref(true),
            right3: ref(false),
            left4: ref(true),
            right4: ref(false),
            left5: ref(true),
            right5: ref(false),
            left6: ref(true),
            right6: ref(false),
            left7: ref(true),
            right7: ref(false),
            left8: ref(true),
            right8: ref(false),
            left9: ref(true),
            right9: ref(false),
        };
    },
    components: { Shopcards }
}
</script>
<style lang="scss" scoped>
  .chekbox{
    opacity: 0.8;
  }
  .chekbox:hover{
    opacity: 1;
    transition: 0.8s;
    color: red;
  }
  .btn{
    opacity: 1;
    transition: 0.8s;
  }
  .btn:hover{
    opacity: 1;
    transition: 1s;
    background-color: red;
    color: white;
  }
  .text-black{
    opacity: 0.8;
  }
  .text-black:hover{
    opacity: 1;
    transition: 1s;
    color: red;
  }
</style>
