<template >
  <div class="q-mt-lg q-mb-xl">
    <div class="w-100pr h-60px ">
      <div class="text-h5">
        Latest Blogs
      </div>
      <div class="text-grey">
        Present posts in a best way to highlight interesting moments of your blog.
      </div>
    </div>
    <div class="w-100pr h-350px row  justify-between items-start content-start">
      <div class="w-32pr h-300px q-mt-lg bg-grey-2 row justify-center content-center" v-for="cart in carts" :key="cart">
        <div class="w-90pr h-80pr bg-grey-2 ">
          <q-btn rounded class="btn text-weight-regular" color="black" :label="cart.btn" />
          <div class="q-mt-lg text-weight-bold fs-16px">
            {{ cart.post }}
          </div>
          <div class="q-mt-md text-grey-8">
            {{ cart.text }}
          </div>
          <div class="q-mt-xl">
            <a class="a " href="">{{ cart.a }}</a>
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
      carts: [
        {
          id: 1,
          btn: 'Organik',
          post: 'This Is Secound Post For XipBlog',
          text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Blanditiis sequi quae enim! Quo consequuntur velit dolores voluptas',
          a: 'Read More'
        },
        {
          id: 1,
          btn: 'Organik',
          post: 'This Is Secound Post For XipBlog',
          text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Blanditiis sequi quae enim! Quo consequuntur velit dolores voluptas',
          a: 'Read More'
        },
        {
          id: 1,
          btn: 'Organik',
          post: 'This Is Secound Post For XipBlog',
          text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Blanditiis sequi quae enim! Quo consequuntur velit dolores voluptas',
          a: 'Read More'
        },
      ]
    }
  },
}
</script>
<style scoped>
.btn {
  padding: 5px 20px;
  font-size: 11px;
}

.a {
  text-decoration: none;
  color: grey;
}
.a:hover{
  margin-left: 10px;
  color: green;
  transition: 1s;
}
</style>
