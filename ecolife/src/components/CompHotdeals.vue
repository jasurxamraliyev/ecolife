<template >
  <div>
      <div class="w-100pr h-950px  row  justify-between items-start content-start">
          <div class="carusel w-35pr h-90pr bg-grey-1">
             <div class="w-100pr h-7pr bg-white">
                 <div class="text-h5">
                      Hot Deals
                  </div>
                  <div class="text-grey">
                      Add hot products to weekly line up
                  </div>
              </div>
              <CompCarusel2/>
          </div>

          <div class="w-63pr h-95pr   row wrap justify-between items-start content-start">
              <div class="w-100pr h-7pr bg-white">
                <div class="text-h5">
                  New Arrivals
                </div>
                <div class="text-grey">
                  Add new products to weekly line upf
                </div>
              </div>
             <div class="cart w-205px h-380px  q-mt-md row justify-center content-center"
                v-for="cart in cart" :key="cart">
                <div class="w-90pr h-90pr  ">
                    <div class="w-100pr h-54pr ">
                      <img :src="cart.img"
                       alt="" class="w-100pr h-97pr">
                    </div>
                    <div class="text w-90pr h-30pr mt-20px ml-10px bg-white">
                        <a class="a fs-12px text-grey" href="">{{cart.href}}</a><br>
                        <a class="a text-subtitle1 text-weight-bold text-black" href="">{{cart.a}}</a>
                      <div class="row items-center">
                          <q-icon :name="cart.icon" color="yellow" size="17px" />
                          <q-icon :name="cart.icon" color="yellow" size="17px" />
                          <q-icon :name="cart.icon" color="yellow" size="17px" />
                          <q-icon :name="cart.icon" color="yellow" size="17px" />
                          <q-icon :name="cart.icon" color="yellow" size="17px" />
                      </div>
                      <div>
                      <del class="text-grey">{{cart.del}}</del>
                       <span class="ml-5px text-dark text-subtitle1">{{cart.span}}</span>
                     </div>
                    </div>
                </div>
             </div>
         </div>
      </div>
  </div>
</template>
<script>
import CompCarusel2 from './CompCarusel2.vue';
export default {
    components: {
    CompCarusel2
  },
  data() {
    return {
      cart:[
        {
          id:1,
          img:'http://demo.posthemes.com/pos_ecolife/layout2/89-home_default/juicy-couture-juicy-quilted-terry-track-jacket.jpg',
          href:'SDUDIO DECIGN',
          a:'Juicy Couture Juicy...',
          icon:'star',
          del:'$35.90',
          span:'$34.11'
        },
        {
          id:1,
          img:'http://demo.posthemes.com/pos_ecolife/layout2/89-home_default/juicy-couture-juicy-quilted-terry-track-jacket.jpg',
          href:'SDUDIO DECIGN',
          a:'Juicy Couture Juicy...',
          icon:'star',
          del:'$35.90',
          span:'$34.11'
        },
        {
          id:1,
          img:'http://demo.posthemes.com/pos_ecolife/layout2/89-home_default/juicy-couture-juicy-quilted-terry-track-jacket.jpg',
          href:'SDUDIO DECIGN',
          a:'Juicy Couture Juicy...',
          icon:'star',
          del:'$35.90',
          span:'$34.11'
        },
        {
          id:1,
          img:'http://demo.posthemes.com/pos_ecolife/layout2/89-home_default/juicy-couture-juicy-quilted-terry-track-jacket.jpg',
          href:'SDUDIO DECIGN',
          a:'Juicy Couture Juicy...',
          icon:'star',
          del:'$35.90',
          span:'$34.11'
        },
        {
          id:1,
          img:'http://demo.posthemes.com/pos_ecolife/layout2/89-home_default/juicy-couture-juicy-quilted-terry-track-jacket.jpg',
          href:'SDUDIO DECIGN',
          a:'Juicy Couture Juicy...',
          icon:'star',
          del:'$35.90',
          span:'$34.11'
        },
        {
          id:1,
          img:'http://demo.posthemes.com/pos_ecolife/layout2/89-home_default/juicy-couture-juicy-quilted-terry-track-jacket.jpg',
          href:'SDUDIO DECIGN',
          a:'Juicy Couture Juicy...',
          icon:'star',
          del:'$35.90',
          span:'$34.11'
        },
        {
          id:1,
          img:'http://demo.posthemes.com/pos_ecolife/layout2/89-home_default/juicy-couture-juicy-quilted-terry-track-jacket.jpg',
          href:'SDUDIO DECIGN',
          a:'Juicy Couture Juicy...',
          icon:'star',
          del:'$35.90',
          span:'$34.11'
        },
        {
          id:1,
          img:'http://demo.posthemes.com/pos_ecolife/layout2/89-home_default/juicy-couture-juicy-quilted-terry-track-jacket.jpg',
          href:'SDUDIO DECIGN',
          a:'Juicy Couture Juicy...',
          icon:'star',
          del:'$35.90',
          span:'$34.11'
        },
      ]
    }
  },
}

</script>
<style scoped>
.text{
line-height: 2.3;
}
.carusel{
  border: 2px solid green;
}
.cart{
  border: 1px solid rgb(229, 228, 228);
}
.a{
 text-decoration: none;
}
</style>
