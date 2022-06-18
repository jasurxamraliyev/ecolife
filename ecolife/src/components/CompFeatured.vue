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
      <div class=" cart w-24pr h-40pr  mt-22px row justify-center content-center" v-for="cart in carts" :key="cart.id">
        <div class="w-93pr h-90pr row  justify-between items-center content-center">
          <div class="w-41pr h-77pr">
            <q-img class="w-90pr h-100pr" :src="cart.src" alt="">
              <div class="search w-100pr h-100pr row content-center justify-center" style="background: none;">
                <q-icon class="icon" size="25px" name="search" />
              </div>
            </q-img>
          </div>
          <div class="text w-55pr h-77pr">
            <div>
              <a class="a fs-12px " href="">{{ cart.studio }}</a>
            </div>
            <div>
              <a class="href text-subtitle1 text-weight-bold text-black" href="">{{ cart.juicy }}</a>
            </div>
            <div class="row items-center">
              <q-icon :name="cart.icon" color="yellow" size="17px" />
              <q-icon :name="cart.icon" color="yellow" size="17px" />
              <q-icon :name="cart.icon" color="yellow" size="17px" />
              <q-icon :name="cart.icon" color="yellow" size="17px" />
              <q-icon :name="cart.icon" color="yellow" size="17px" />
            </div>
            <div>
              <del class="text-grey">{{ cart.del }}</del>
              <span class="ml-5px text-dark text-subtitle1">{{ cart.span }}</span>
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
      carts: [
        {
          id: 1,
          src: 'http://demo.posthemes.com/pos_ecolife_fastfood/375-home_default/pizza-mushrooms.jpg',
          studio: 'SDUDIO DECIGN',
          juicy: 'Juicy Couture Juicy...',
          icon: 'star',
          del: '$35.90',
          span: '$34.11'
        },
        {
          id: 2,
          src: 'http://demo.posthemes.com/pos_ecolife_fastfood/375-home_default/pizza-mushrooms.jpg',
          studio: 'SDUDIO DECIGN',
          juicy: 'Juicy Couture Juicy...',
          icon: 'star',
          del: '$35.90',
          span: '$34.11'
        },
        {
          id: 3,
          src: 'http://demo.posthemes.com/pos_ecolife_fastfood/375-home_default/pizza-mushrooms.jpg',
          studio: 'SDUDIO DECIGN',
          juicy: 'Juicy Couture Juicy...',
          icon: 'star',
          del: '$35.90',
          span: '$34.11'
        },
        {
          id: 4,
          src: 'http://demo.posthemes.com/pos_ecolife_fastfood/375-home_default/pizza-mushrooms.jpg',
          studio: 'SDUDIO DECIGN',
          juicy: 'Juicy Couture Juicy...',
          icon: 'star',
          del: '$35.90',
          span: '$34.11'
        },
        {
          id: 5,
          src: 'http://demo.posthemes.com/pos_ecolife_fastfood/375-home_default/pizza-mushrooms.jpg',
          studio: 'SDUDIO DECIGN',
          juicy: 'Juicy Couture Juicy...',
          icon: 'star',
          del: '$35.90',
          span: '$34.11'
        },
        {
          id: 6,
          src: 'http://demo.posthemes.com/pos_ecolife_fastfood/375-home_default/pizza-mushrooms.jpg',
          studio: 'SDUDIO DECIGN',
          juicy: 'Juicy Couture Juicy...',
          icon: 'star',
          del: '$35.90',
          span: '$34.11'
        },
        {
          id: 7,
          src: 'http://demo.posthemes.com/pos_ecolife_fastfood/375-home_default/pizza-mushrooms.jpg',
          studio: 'SDUDIO DECIGN',
          juicy: 'Juicy Couture Juicy...',
          icon: 'star',
          del: '$35.90',
          span: '$34.11'
        },
        {
          id: 8,
          src: 'http://demo.posthemes.com/pos_ecolife_fastfood/375-home_default/pizza-mushrooms.jpg',
          studio: 'SDUDIO DECIGN',
          juicy: 'Juicy Couture Juicy...',
          icon: 'star',
          del: '$35.90',
          span: '$34.11'
        },
      ]
    }
  },
}
</script>
<style scoped>
.cart {
  border: 1px solid rgb(229, 228, 228);
}

.href {
  text-decoration: none;
}

.a {
  text-decoration: none;
  color: grey;
}

.a:hover {
  margin-left: 10px;
  color: green;
  transition: 1s;
}

.text {
  line-height: 2;
}

.cart:hover {
  border: 2px solid green;
}

.search {
  opacity: 0;
}

.search:hover {
  opacity: 1;
}

.icon {
  background-color: #fff;
  border-radius: 22px;
  padding: 10px;
  color: grey;
}

.icon:hover {
  background-color: red;
  color: #fff;
  transition: 1s;
}
</style>
