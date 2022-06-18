<template >
  <div>
    <div class="w-100pr h-950px  row  justify-between items-start content-start">
      <div class=" w-35pr h-90pr bg-grey-1">
        <div class="w-100pr h-7pr bg-white">
          <div class="text-h5">
            Hot Deals
          </div>
          <div class="text-grey">
            Add hot products to weekly line up
          </div>
        </div>
        <CompCarusel2 />
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
        <div class="cart w-205px h-380px  q-mt-md row justify-center content-center" v-for="cart in cart"
          :key="cart.id">
          <div class="w-90pr h-90pr  ">
            <div class="w-100pr h-54pr ">
              <q-img :src="cart.img" alt="" class="img w-100pr h-97pr">
                <div class="search w-100pr h-100pr row content-center justify-center" style="background: none;">
                  <q-icon class="icon" size="25px" name="search" />
                </div>
              </q-img>
            </div>
            <div class="text w-90pr h-30pr mt-20px ml-10px ">
              <a class="href fs-12px " href="">{{ cart.href }}</a><br>
              <a class="a text-subtitle1 text-weight-bold text-black" href="">{{ cart.a }}</a>
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
      cart: [
        {
          id: 1,
          img: 'http://demo.posthemes.com/pos_ecolife_fastfood/375-home_default/pizza-mushrooms.jpg',
          href: 'SDUDIO DECIGN',
          a: 'Juicy Couture Juicy...',
          icon: 'star',
          del: '$35.90',
          span: '$34.11'
        },
        {
          id: 2,
          img: 'http://demo.posthemes.com/pos_ecolife_fastfood/375-home_default/pizza-mushrooms.jpg',
          href: 'SDUDIO DECIGN',
          a: 'Juicy Couture Juicy...',
          icon: 'star',
          del: '$35.90',
          span: '$34.11'
        },
        {
          id: 3,
          img: 'http://demo.posthemes.com/pos_ecolife_fastfood/375-home_default/pizza-mushrooms.jpg',
          href: 'SDUDIO DECIGN',
          a: 'Juicy Couture Juicy...',
          icon: 'star',
          del: '$35.90',
          span: '$34.11'
        },
        {
          id: 4,
          img: 'http://demo.posthemes.com/pos_ecolife_fastfood/375-home_default/pizza-mushrooms.jpg',
          href: 'SDUDIO DECIGN',
          a: 'Juicy Couture Juicy...',
          icon: 'star',
          del: '$35.90',
          span: '$34.11'
        },
        {
          id: 5,
          img: 'http://demo.posthemes.com/pos_ecolife_fastfood/375-home_default/pizza-mushrooms.jpg',
          href: 'SDUDIO DECIGN',
          a: 'Juicy Couture Juicy...',
          icon: 'star',
          del: '$35.90',
          span: '$34.11'
        },
        {
          id: 6,
          img: 'http://demo.posthemes.com/pos_ecolife_fastfood/375-home_default/pizza-mushrooms.jpg',
          href: 'SDUDIO DECIGN',
          a: 'Juicy Couture Juicy...',
          icon: 'star',
          del: '$35.90',
          span: '$34.11'
        },
        {
          id: 7,
          img: 'http://demo.posthemes.com/pos_ecolife_fastfood/375-home_default/pizza-mushrooms.jpg',
          href: 'SDUDIO DECIGN',
          a: 'Juicy Couture Juicy...',
          icon: 'star',
          del: '$35.90',
          span: '$34.11'
        },
        {
          id: 8,
          img: 'http://demo.posthemes.com/pos_ecolife_fastfood/375-home_default/pizza-mushrooms.jpg',
          href: 'SDUDIO DECIGN',
          a: 'Juicy Couture Juicy...',
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
.text {
  line-height: 2.3;
}

.cart {
  border: 1px solid rgb(229, 228, 228);
}

.a {
  text-decoration: none;
}

.href {
  text-decoration: none;
  color: grey;
}

.href:hover {
  margin-left: 10px;
  color: green;
  transition: 1s;
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
