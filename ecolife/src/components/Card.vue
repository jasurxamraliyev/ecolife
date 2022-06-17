<template>
  <div class="w-100pr">
    <div class="text-h6  ml-75px">
      Shopping Cart
    </div>
    <div  v-for="card in cards" :key="card" class="w-55pr ml-75px mt-50px h-120px">
      <div class=" w-100pr h-100pr row items-center">
        <div class="w-25pr ">
          <q-img width=" 50%" :src="card.src" />
        </div>
        <div class="w-25pr h-90pr" >
          <div class="fs-16px">
            {{card.span}}
          </div>
          <div>
            <span class="mr-5pr text-red-9">{{card.number}}</span> <del class="mr-5pr">{{card.del}}</del>
            <span class="bg-black text-white pl-5px pr-5px p-3px">{{card.num}}</span>
          </div>
        </div>
        <div class="w-17pr h-90pr row justify-center">
            <span class="fs-18px">+ 5 -</span>
        </div>
        <div class="w-17pr h-90pr row justify-center">
          <span class="fs-16px">{{card.iq}}</span>
        </div>
        <div class="w-13pr h-90pr row justify-end">
          <q-icon size="22px" :name="card.icon" />
        </div>
      </div>
      <q-separator class=" w-100pr" color="grey-5" size="2px"  />
    </div>
      <div class="mt-2pr ml-4pr">
        <q-btn class="btn"   label="Continue Shopping" />
      </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      cards: [
        {
          src: 'http://demo.posthemes.com/pos_ecolife_fastfood/375-cart_default/pizza-mushrooms.jpg',
          span: ' Pizza Mushrooms',
          number: '$21.51 ',
          del: '$23.90',
          num: '-10%',
          iq: '$21.51',
          icon: 'delete',

        },
        {
          src: 'http://demo.posthemes.com/pos_ecolife_fastfood/375-cart_default/pizza-mushrooms.jpg',
          span: ' Pizza Mushrooms',
          number: '$21.51 ',
          del: '$23.90',
          num: '-10%',
          iq: '$21.51',
          icon: 'delete',

        },
        {
          src: 'http://demo.posthemes.com/pos_ecolife_fastfood/375-cart_default/pizza-mushrooms.jpg',
          span: ' Pizza Mushrooms',
          number: '$21.51 ',
          del: '$23.90',
          num: '-10%',
          iq: '$21.51',
          icon: 'delete',

        },
        {
          src: 'http://demo.posthemes.com/pos_ecolife_fastfood/375-cart_default/pizza-mushrooms.jpg',
          span: ' Pizza Mushrooms',
          number: '$21.51 ',
          del: '$23.90',
          num: '-10%',
          iq: '$21.51',
          icon: 'delete',

        },

      ]
    }
  }
}
</script>

<style scoped>
.btn{
  background-color: black;
  transition: 0.6s ease ;
  color: white;
}
.btn:hover{
  background-color: red;

}

</style>
