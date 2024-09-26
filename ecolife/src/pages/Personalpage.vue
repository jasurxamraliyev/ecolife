<template> 
  <div> 
    <br><br> 
    <!--responsive 1 --> 
    <div class="fit row justify-around"> 
      <div class=" md w-45pr mobile-hide"> 
        <comp-personal /> 
      </div> 
      <div class=" md w-30pr q-mt-xl q-ml-xl"> 
        <comp-totel /> 
      </div> 
    </div> 
    <!--responsive 2 --> 
    <div> 
      <div class=" justify-around  row xs w-100pr "> 
        <div class="w-90pr"> 
          <comp-personal /> 
        </div> 
      </div> 
      <div class="row justify-around xs w-100pr q-mt-xl"> 
        <div class="w-90pr"> 
          <comp-totel /> 
        </div> 
 
      </div> 
    </div> 
    <!--responsive 3 --> 
    <div class="fit row justify-around"> 
      <div class=" sm w-45pr "> 
        <comp-personal /> 
      </div> 
      <div class=" sm w-43pr q-mt-xl"> 
        <comp-totel />  
      </div> 
    </div> 
    <!-- responsive 4 --> 
     <div class="fit  row justify-around"> 
      <div class=" lg w-40pr mobile-hide"> 
        <comp-personal /> 
      </div> 
      <div class=" lg w-23pr q-mt-xl"> 
       <comp-totel /> 
      </div> 
    </div> 
    <!-- reponsive5 -->
    <div class="fit  row justify-around"> 
      <div class=" xl w-40pr mobile-hide"> 
        <comp-personal /> 
      </div> 
      <div class=" xl w-23pr q-mt-xl"> 
       <comp-totel /> 
      </div> 
    </div> 
    <br><br> 
 
  </div> 
</template> 
 
<script> 
import CompPersonal from '../components/CompPersonal.vue'
import CompTotel from '../components/CompTotel.vue'

 
export default {
  components: { CompPersonal, CompTotel }, 
  
 
} 
</script> 
 
<style> 
</style>