<template >
  <div>
    <div>
      <CompCarusel />
    </div>
    <div class="mt-340px"></div>
    <div class="container row wrap justify-center">
      <div class="content">
        <CompPopular />
        <CompHotdeals />
      </div>
    </div>

    <div class="w-100pr h-460px row">
      <div class="w-50pr h-100pr">
        <q-img src="http://demo.posthemes.com/pos_ecolife_fastfood/img/cms/5_1.jpg" />
      </div>
      <div class="w-50pr h-100pr">
        <q-img src="http://demo.posthemes.com/pos_ecolife_fastfood/img/cms/6_1.jpg" />
      </div>
    </div>

    <div class="container row wrap justify-center">
      <div class="content">
        <CompFeatured />
        <CompLatest />
      </div>
    </div>
  </div>
</template>

<script>
import CompCarusel from "src/components/CompCarusel";
import CompPopular from "../components/CompPopular";
import CompFeatured from "src/components/CompFeatured";
import CompLatest from "src/components/CompLatest";
import CompHotdeals from "src/components/CompHotdeals.vue";
export default {
  components: {
    CompCarusel,
    CompPopular,
    CompFeatured,
    CompLatest,
    CompHotdeals,
  },
};
</script>
<style>
.container {
  width: 100%;
  height: auto;
}

.content {
  width: 92%;
  height: 93%;
}
</style>
