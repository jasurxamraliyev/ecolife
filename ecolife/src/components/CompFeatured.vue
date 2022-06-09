<template>
  <div class="q-mt-xl">
    <div class="w-100pr h-70px  content-center">
      <div class="text-h5 mt-10px">
         Featured Products
      </div>
      <div class="text-grey ">
         Add featured products to weekly line up
      </div>
    </div>

    <div class="w-100pr h-433px bg-white  row wrap justify-between items-start content-start">
        <div class=" cart w-24pr h-40pr  mt-22px row justify-center content-center"
            v-for="cart in carts"
            :key="cart">
            <div class="w-93pr h-90pr row  justify-between items-center content-center">
                <div class="w-41pr h-77pr">
                    <img class="w-90pr h-100pr"
                     :src="cart.src" alt="">
                </div>
                <div class="text w-55pr h-77pr">
                   <div>
                      <a class="a fs-12px text-grey"
                       href="">{{cart.studio}}</a>
                   </div>
                    <div>
                      <a class="a text-subtitle1 text-weight-bold text-black"
                       href="">{{cart.juicy}}</a>
                    </div>
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
</template>
<script>
export default {
    data() {
      return {
        carts:[
          {
            id:1,
            src:'http://demo.posthemes.com/pos_ecolife/layout2/89-home_default/juicy-couture-juicy-quilted-terry-track-jacket.jpg',
            studio:'SDUDIO DECIGN',
            juicy:'Juicy Couture Juicy...',
            icon:'star',
            del:'$35.90',
            span:'$34.11'
          },
          {
            id:2,
            src:'http://demo.posthemes.com/pos_ecolife/layout2/89-home_default/juicy-couture-juicy-quilted-terry-track-jacket.jpg',
            studio:'SDUDIO DECIGN',
            juicy:'Juicy Couture Juicy...',
            icon:'star',
            del:'$35.90',
            span:'$34.11'
          },
          {
            id:3,
            src:'http://demo.posthemes.com/pos_ecolife/layout2/89-home_default/juicy-couture-juicy-quilted-terry-track-jacket.jpg',
            studio:'SDUDIO DECIGN',
            juicy:'Juicy Couture Juicy...',
            icon:'star',
            del:'$35.90',
            span:'$34.11'
          },
          {
            id:4,
            src:'http://demo.posthemes.com/pos_ecolife/layout2/89-home_default/juicy-couture-juicy-quilted-terry-track-jacket.jpg',
            studio:'SDUDIO DECIGN',
            juicy:'Juicy Couture Juicy...',
            icon:'star',
            del:'$35.90',
            span:'$34.11'
          },
          {
            id:5,
            src:'http://demo.posthemes.com/pos_ecolife/layout2/89-home_default/juicy-couture-juicy-quilted-terry-track-jacket.jpg',
            studio:'SDUDIO DECIGN',
            juicy:'Juicy Couture Juicy...',
            icon:'star',
            del:'$35.90',
            span:'$34.11'
          },
          {
            id:6,
            src:'http://demo.posthemes.com/pos_ecolife/layout2/89-home_default/juicy-couture-juicy-quilted-terry-track-jacket.jpg',
            studio:'SDUDIO DECIGN',
            juicy:'Juicy Couture Juicy...',
            icon:'star',
            del:'$35.90',
            span:'$34.11'
          },
          {
            id:7,
            src:'http://demo.posthemes.com/pos_ecolife/layout2/89-home_default/juicy-couture-juicy-quilted-terry-track-jacket.jpg',
            studio:'SDUDIO DECIGN',
            juicy:'Juicy Couture Juicy...',
            icon:'star',
            del:'$35.90',
            span:'$34.11'
          },
          {
            id:8,
            src:'http://demo.posthemes.com/pos_ecolife/layout2/89-home_default/juicy-couture-juicy-quilted-terry-track-jacket.jpg',
            studio:'SDUDIO DECIGN',
            juicy:'Juicy Couture Juicy...',
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
.cart{
  border: 1px solid rgb(229, 228, 228);
}
.a{
 text-decoration: none;
}
.text{
 line-height: 2;
}

</style>
