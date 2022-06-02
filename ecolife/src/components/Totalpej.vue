<template>
  <div class="container  shadow-up-14">
        <div class="contier ">
          <div class="q-ml-sm q-mr-sm text-subtitle2">2 items</div>
              <q-list class="rounded-borders"/>
              <q-expansion-item
                expand-separator label="show details">
                <q-card>
                  <q-card-section>
                    <div>Originals Kaval Windbreaker Winte</div>
                    <div>Jacket 2</div>
                    <div>x1</div>
                    <div class="row justify-between">
                      <div>Size: S</div>
                      <div style="color:blueviolet">$21.51</div>
                    </div>
                  </q-card-section>
                </q-card>
              </q-expansion-item>
            <div class="row justify-between  text-subtitle2 q-ml-sm q-mr-sm">
              <div>Subtotal</div>
              <div >$33.41</div>
            </div>
            <div class="row justify-between text-subtitle2 q-ml-sm q-mr-sm">
              <div>Shipping</div>
              <div>$7.00</div>
            </div><br>
        </div>
        <div class="row justify-between text-subtitle2 q-ml-sm q-mr-sm">
          <div>Total (Tax Excl.)</div>
          <div>$40.41</div>
        </div>
        <div class="row justify-between text-subtitle2 q-ml-sm q-mr-sm">
          <div>Taxes</div>
          <div>$0.00</div>
        </div><br>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
  .container{
    width: 240px;
    height: auto;
    /* box-shadow: 2px 3px rgb(122, 117, 117); */
    border-radius: 8px;
  }
  .btn{
    border: none;
  }
  .contier{
    width: 100%;
    border-bottom: 1px solid grey;
  }


</style>
