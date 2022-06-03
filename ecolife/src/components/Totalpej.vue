<template>
  <div class="container w-300px br-6px shadow-up-14">
        <div class="contier w-100pr q-pt-sm">
          <div class="q-ml-sm  q-mr-sm text-subtitle2">2 items</div>
              <q-list class="rounded-borders"/>
              <q-expansion-item
                expand-separator label="show details">
                <q-card>
                  <q-card-section>
                    <div>Originals Kaval Windbreaker Winte Jacket 2</div>
                    <div>x1</div>

                    <div class="row justify-between">
                      <div>Size: S</div>
                      <div style="color:blueviolet">$21.51</div>
                    </div>

                    <div class="q-mt-md">
                      <div>Trans-Weight Hooded Wind and Water Resistant Shell</div>
                      <div class="row justify-between q-mt-sm">
                        <div>x1</div>
                        <div style="color:blueviolet">$11.90</div>
                      </div>
                    </div>
                  </q-card-section>
                </q-card>
              </q-expansion-item>
            <div class="row justify-between  text-subtitle2 q-ml-sm q-mr-sm">
              <div>Subtotal</div>
              <div >$33.41</div>
            </div>
            <div :key="suma" class="row justify-between text-subtitle2 q-ml-sm q-mr-sm">
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
  .btn{
    border: none;
  }
  .contier{
    border-bottom: 1px solid grey;
  }
</style>
