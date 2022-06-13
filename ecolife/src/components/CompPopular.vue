<template>
  <div>
    <div class="w-100pr h-80px bg-white q-mt-lg row content-center">
      <div>
        <div class="text-h5">Popular Categories</div>
        <div class="text-grey">Add Popular Categories to weekly line up</div>
      </div>
    </div>

    <div
      class="
        w-100pr
        h-430px
        bg-white
        row
        wrap
        justify-between
        items-start
        content-start
      "
    >
      <div class="w-32pr h-32 q-mt-lg" v-for="cart in carts" :key="cart">
        <q-img class="w-32r h-32" :src="cart.img">
          <div
            class="w-100pr h-100pr row items-center"
            style="background: none"
          >
            <div
              class="text-fresh q-ml-md w-40pr h-70pr"
              style="background: none"
            >
              <div class="text-h6 text-weight-medium text-black">
                {{ cart.fresh }}
              </div>
              <div class="text-grey">
                {{ cart.product }}
              </div>
              <div class="a">
                <a href="">{{ cart.a }}</a>
              </div>
            </div>
          </div>
        </q-img>
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
          img: "http://demo.posthemes.com/pos_ecolife/layout2/modules/poslistcategories/images/thumb-3.jpg",
          fresh: " Fresh Vegetables",
          product: "17 Product",
          a: "Shop Now",
        },
        {
          id: 1,
          img: "http://demo.posthemes.com/pos_ecolife/layout2/modules/poslistcategories/images/thumb-3.jpg",
          fresh: " Fresh Vegetables",
          product: "17 Product",
          a: "Shop Now",
        },
        {
          id: 1,
          img: "http://demo.posthemes.com/pos_ecolife/layout2/modules/poslistcategories/images/thumb-3.jpg",
          fresh: " Fresh Vegetables",
          product: "17 Product",
          a: "Shop Now",
        },
        {
          id: 1,
          img: "http://demo.posthemes.com/pos_ecolife/layout2/modules/poslistcategories/images/thumb-3.jpg",
          fresh: " Fresh Vegetables",
          product: "17 Product",
          a: "Shop Now",
        },
        {
          id: 1,
          img: "http://demo.posthemes.com/pos_ecolife/layout2/modules/poslistcategories/images/thumb-3.jpg",
          fresh: " Fresh Vegetables",
          product: "17 Product",
          a: "Shop Now",
        },
        {
          id: 1,
          img: "http://demo.posthemes.com/pos_ecolife/layout2/modules/poslistcategories/images/thumb-3.jpg",
          fresh: " Fresh Vegetables",
          product: "17 Product",
          a: "Shop Now",
        },
      ],
    };
  },
};
</script>
<style scoped>
a {
  text-decoration: none;
  color: rgb(83, 81, 81);
  font-size: 14px;
}
.text-fresh {
  line-height: 2;
}
.a a:hover {
  margin-left: 10px;
  color: green;
  transition: 1s;
}
</style>
