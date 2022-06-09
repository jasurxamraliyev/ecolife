<template >
  <div>
    <CompCarusel/>
    <div class="container row wrap justify-center">
      <div class="content ">
           <CompImg/>
           <CompPopular/>
          <CompHotdeals/>
      </div>
    </div>
    <div>
        <q-img class="img w-100pr h-400px" src="http://demo.posthemes.com/pos_ecolife/layout2/modules/posslideshows/images/081b9c1b802e10a8438349ca084ec5451f955c8e_2_2.jpg">

        </q-img>
    </div>
    <div class="container row wrap justify-center">
      <div class="content">
         <CompFeatured/>
          <CompWemake/>
          <CompLatest/>
     </div>
    </div>
  </div>
</template>
<script>
import CompCarusel from 'src/components/CompCarusel';
import CompImg from 'src/components/CompImg';
import CompPopular from '../components/CompPopular';
import CompFeatured from 'src/components/CompFeatured';
import CompLatest from 'src/components/CompLatest';
import CompWemake from 'src/components/CompWemake.vue';
import CompHotdeals from 'src/components/CompHotdeals.vue';
export default {
    components: {
    CompCarusel,
    CompImg,
    CompPopular,
    CompFeatured,
    CompLatest,
    CompWemake,
    CompHotdeals
}
}
</script>
<style>
.container{
  width: 100%;
  height: auto;
}
.content{
  width: 92%;
  height: 93%;
}

</style>
