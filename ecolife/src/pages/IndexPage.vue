<template >
  <div>
    <CompCarusel/>
    <div class="container   row wrap justify-center">
      <div class="content bg-grey">
           <CompImg/>
           <!-- <CompPopular/> -->
           <!-- <CompFeatured/> -->
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
export default {
    components: {
    CompCarusel,
    CompImg,
    CompPopular,
    CompFeatured,
    CompLatest
}
}
</script>
<style>
.container{
  width: 100%;
  height: 1000px;
}
.content{
  width: 1421px;
  height: 1000px;
}
</style>
