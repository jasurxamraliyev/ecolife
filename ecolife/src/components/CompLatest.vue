<template >
  <div>
    <div class="w-100pr h-60px bg-red">
        <div class="text-h5">
          Latest Blogs
        </div>
        <div>
          Present posts in a best way to highlight interesting moments of your blog.
        </div>
    </div>
    <div class="w-100pr h-350px bg-blue">
        <div class="w-32pr h-300px bg-yellow row justify-center content-center">
            <div class="w-90pr h-80pr bg-grey-2 ">
                 <q-btn  rounded  class="btn text-weight-regular" color="black" label="Organik" />
                 <div class="q-mt-lg text-weight-bold fs-16px">
                    This Is Secound Post For XipBlog
                 </div>
                 <div class="q-mt-md">
                   Lorem ipsum dolor sit amet consectetur adipisicing elit. Blanditiis sequi quae enim! Quo consequuntur velit dolores voluptas
                 </div>
                 <div class="q-mt-xl">
                   <a class="a" href="">Read More</a>
                 </div>
            </div>
        </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {

    }
  },
}
</script>
<style scoped>
.btn{
  padding: 5px 20px ;
  font-size: 11px;
}
.a{
  text-decoration: none;
}
</style>
