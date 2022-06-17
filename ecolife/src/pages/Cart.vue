<template>
  <q-page>
    <div class="row w-100pr justify-around mt-5pr" >
      <div class="w-70pr">
      <card />
    </div>
      <div class="w-20pr ">
        <card2  />
      </div>
    </div>

  </q-page>
</template>

<script>
import Card from '../components/Card.vue'
import Card2 from 'src/components/Card2.vue'
export default {
  components: { Card, Card2 },

}
</script>

<style>

</style>
