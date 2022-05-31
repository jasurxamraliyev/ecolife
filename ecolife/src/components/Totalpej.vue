<template>
  <div class="container bg-grey-1">
        <div class="contier">
          <div>2 items</div>
          <q-btn-dropdown outline flat  class="btn" color="primary" label="Dropdown Button">
              <q-list>
                <q-item >
                  <q-item-section>
                    <q-item-label>












                    </q-item-label>
                  </q-item-section>
                </q-item>
              </q-list>
            </q-btn-dropdown>
            <div class="row">
              <div>Subtotal</div>
              <div >$33.41</div>
            </div>
            <div class="row">
              <div>Shipping</div>
              <div>$7.00</div>
            </div>
        </div>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
  .container{
    width: 300px;
    height: 230px;
    border: 1px solid gray;
  }
  .btn{
    border: none;
  }
  .contier{
    width: 100%;
    border-bottom: 1px solid grey;
  }
</style>
