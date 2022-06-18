<template> 
  <div> 
    <!-- bosh sarlavha --> 
    <div 
      class=" 
        w-100pr 
        container 
        br-10px 
        w-81pr 
        row 
        justify-center 
        content-center 
        shadow-up-14 
        q-pb-xl 
      " 
    > 
      <div class="w-100pr h-550px q-ml-md items-center"> 
        <br /> 
        <div class=" text-grey contact text-h5 text-weight-bolder"> 
          1 Personal Information 
        </div> 
        <!-- inputlar boshlanishi --> 
        <br /> 
        <form> 
          <div class="q-mt-xl q-ml-md items-start content-start"> 
            <q-input 
              type="text" 
              class="w-90pr mb-40px" 
              v-model="text" 
              label="Name" 
              :dense="dense" 
            /> 
            <q-input 
              type="text" 
              class="w-90pr mb-40px" 
              v-model="text1" 
              label="Surname" 
              :dense="dense" 
            /> 
          </div> 
        </form> 
 
        <div class="q-mt-xl q-ml-md"> 
          <form> 
            <q-input 
              class="w-90pr" 
              type="number" 
              v-model="number" 
              label="Number" 
              :dense="dense" 
            /> 
          </form> 
        </div> 
 
        <div class="q-mt-xl w-90pr q-ml-md"> 
          <form> 
            <q-input 
              type="textarea" 
              v-model="textarea" 
              label="Location" 
              :dense="dense" 
            /> 
          </form> 
        </div> 
        <br /> 
        <div class="row q-mt-md justify-center"> 
          <q-btn color="secondary" label="Send Message" /> 
        </div> 
        <br /><br /> 
        <!-- inputlar tugashi --> 
      </div> 
      <br /> 
    </div> 
    <!-- bosh sarlavha tugashi --> 
  </div> 
</template> 
<script> 
import { ref } from "vue"; 
export default { 
  setup() { 
    return { 
      text: ref(""), 
      text1: ref(""), 
      number: ref(""), 
      textarea: ref(""), 
      dense: ref(true), 
    }; 
  }, 
}; 
</script>