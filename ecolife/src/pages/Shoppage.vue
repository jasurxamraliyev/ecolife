<template>
  <q-page>

    <div class=" row  justify-between mt-2pr">
      <Shoppage/>
    <div class="w-70pr_md-70pr_sm-70pr  ">
      <Shopcards/>
    </div>
    </div>

  </q-page>
</template>
<script>


import Shopcards from 'src/components/Shopcards.vue'
import Shoppage from 'src/components/Shoppage.vue'

export default {
    setup() {

    },
    components: { Shopcards, Shoppage }
}
</script>

<style lang="scss" scoped>
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
