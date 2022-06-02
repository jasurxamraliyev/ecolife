<template>
  <div>
        <!-- bosh sarlavha -->
      <div class="container row justify-center content-center shadow-up-14">
        <div class="content q-ml-md  items-center"><br>
            <div class="contact text-h5 text-weight-bolder">
              1 Personal Information
            </div>
            <!-- inputlar boshlanishi -->
                  <br>
                <form>
                  <div class="q-mt-xl q-ml-md items-start content-start">
                    <q-input type="text" class="input-text" v-model="text" label="Name" :dense="dense" />
                    <q-input  type="text" class="input-text" v-model="text1" label="Surname" :dense="dense" />
                  </div>
                </form>

                <div class="q-mt-xl q-ml-md ">
                  <form>
                    <q-input style="width:90%" type="number"  v-model="number" label="Number" :dense="dense" />
                  </form>
                </div>

               <div class="q-mt-xl inp-1 q-ml-md">
                  <form>
                   <q-input  type="textarea"  v-model="textarea" label="Location" :dense="dense" />
                  </form>
              </div>
                <br>
               <div class=" row justify-center">
                  <q-btn color="secondary" label="Send Message" />
               </div><br><br>
              <!-- inputlar tugashi -->
        </div><br><br>
      </div>
       <!-- bosh sarlavha tugashi -->
  </div>
</template>
<script>
import { ref } from 'vue'
export default {
    setup () {
    return {
      text: ref(''),
      text1: ref(''),
      number: ref(''),
      textarea: ref(''),
      dense: ref(true)
    }
  }
}
</script>
<style scoped>
.container{
  width: 81%;
  height: auto;
  border-radius: 8px;
}
.content{
  width: 650px;
  height: 550px;
}
.input-text{
  width: 90%;
  margin-bottom: 40px;
}
.inp-1{
  width: 90%;
}

</style>
