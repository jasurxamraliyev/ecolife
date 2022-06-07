<template>
  <div><br><br>
   <div class="fit row col-12  justify-around items-star content-start">
      <div class="w-50pr mobile-hide">
        <Persinal/>
      </div>
      <div class="q-mt-xl">
        <Totalpej/>
      </div>
   </div>
    <div class="h-100px">

    </div>
  </div>
</template>

<script>
import Persinal from 'src/components/persinal.vue';
import Totalpej from 'src/components/Totalpej.vue';
export default {
    components: { Persinal, Totalpej }
}
</script>

<style>

</style>
