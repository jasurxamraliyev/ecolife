<template>
  <q-layout view="hhh lpR fff">

    <q-header reveal bordered class="bg-grey-1 h-70px content-center" >
      <q-toolbar>
        <div class="w-15pr h-50px  mt-10px">
           <img src="http://demo.posthemes.com/pos_ecolife/layout2/img/ecolife-responsive-prestashop-theme-logo-1580528177.jpg" alt="">
        </div>
        <div class="row w-85pr h-50px  mt-10px content-center">
            <span class="span q-ml-xl text-subtitle2 text-weight-bold text-black">Home</span>
            <span class="span q-ml-xl text-subtitle2 text-weight-bold text-black">Fresh Food</span>
            <span class="span q-ml-xl text-subtitle2 text-weight-bold text-black">Fresh Vegetable</span>
            <span class="span q-ml-xl text-subtitle2 text-weight-bold text-black">Prices Drop</span>
            <span class="span q-ml-xl text-subtitle2 text-weight-bold text-black">Contact us</span>
            <q-space/>
             <q-icon color="black" size="25px" name="search" class="q-mr-md"/>
             <q-icon color="black" size="25px" name="lock"/><strong class="mt-3px mr-10px text-black text-weight-bold">$0.00</strong>
      </div>

      </q-toolbar>
    </q-header>

    <q-page-container>
      <router-view />
    </q-page-container>

    <q-footer bordered class="bg-grey-8 text-white">
      <q-toolbar>

      </q-toolbar>
    </q-footer>

  </q-layout>
</template>

<script>

</script>

<style>
.span{
  cursor: pointer;
}
</style>
