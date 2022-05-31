<template>
  <div class="fit row  justify-around items-star content-start"><br><br>
    <div class="q-mt-xl">
       <Persinal/>
    </div>
    <div class="q-mt-xl">
       <Totalpej/>
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
