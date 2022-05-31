<template>
  <div>
        <!-- bosh sarlavha -->
      <div class="container row justify-center content-center">
        <div class="content "><br>
            <div class="contact text-h5 text-weight-bolder">
              1 Personal Information
            </div>
            <!-- inputlar boshlanishi -->
                  <br>
                <form>
                  <div class="q-mt-xl row  justify-between items-start content-start">
                    <q-input type="text" class="input-text" v-model="text" label="Name" :dense="dense" />
                    <q-input  type="text" class="input-text" v-model="text" label="Surname" :dense="dense" />
                  </div>
                </form>

                <div class="q-mt-xl ">
                  <form>
                    <q-input style="width:50%" type="number"  v-model="number" label="Number" :dense="dense" />
                  </form>
                </div>

               <div class="q-mt-xl">
                  <form>
                   <q-input  type="textarea"  v-model="textarea" label="Location" :dense="dense" />
                  </form>
              </div>

               <div class="q-mt-xl row justify-end">
                  <q-btn color="secondary" label="Send Message" />
               </div>
              <!-- inputlar tugashi -->
        </div>
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
      text: ref(''),
      number: ref(''),
      textarea: ref(''),
      dense: ref(true)
    }
  }
}
</script>
<style scoped>
.container{
  width: 89%;
  height: 90vh;
  border: 1px solid gray;

}
.content{
  width: 650px;
  height: 550px;
}
.input-text{
  width: 47%;
}
</style>
