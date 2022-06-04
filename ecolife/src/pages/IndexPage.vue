<template >
  <div>
    <CompCarusel/>
    <div class="container  bg-red row wrap justify-center">
      <CompImg/>
    </div>
  </div>
</template>
<script>
import CompCarusel from 'src/components/CompCarusel';
import CompImg from 'src/components/CompImg';
export default {
    components: { CompCarusel, CompImg }
}
</script>
<style>
.container{
  width: 100%;
  height: 1000px;
}
</style>
