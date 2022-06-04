<template>
  <q-layout view="hhh lpR fff">

    <q-header reveal bordered class="bg-grey-1 h-70px content-center" >
      <q-toolbar>
        <div class="w-15pr h-50px bg-red mt-10px">
           <img src="http://demo.posthemes.com/pos_ecolife/layout2/img/ecolife-responsive-prestashop-theme-logo-1580528177.jpg" alt="">
        </div>
        <div class="row w-85pr h-50px bg-blue mt-10px content-center">
            <span class="q-ml-xl">About</span>
            <span class="q-ml-xl">Fresh Food</span>
            <span class="q-ml-xl">Fresh Vegetable</span>
            <span class="q-ml-xl">Prices Drop</span>
            <span class="q-ml-xl">Contact us</span>
            <q-space/>
             <q-icon  name="lock"/>
             <q-icon name="search" class="q-ml-md"/>
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
