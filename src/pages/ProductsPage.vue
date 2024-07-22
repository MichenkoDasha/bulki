<template>
    <q-page-container>
      <div class="q-pa-md">
        <div class="row justify-center q-gutter-md">

            <q-card flat bordered class="my-card q-ma-lg">
              <img src="~assets/bread1.jpg" alt="" />

              <q-card-section>
                <div class="text-h6">Хлеб пшеничный</div>
                <div class="text-subtitle2">
                  Мука пшеничная в/с, мука пшеничная ц/з, вода, соль, мука рисовая.</div>
              </q-card-section>
            </q-card>
          <q-card flat bordered class="my-card q-ma-lg">
            <img src="~assets/bread2.jpg" alt="" />

            <q-card-section>
              <div class="text-h6">Багет хрустящий</div>
              <div class="text-subtitle2">Мука пшеничная в/с, вода питьевая, соль, дрожжи хлебопекарные прессованные, мука рисовая.</div>
            </q-card-section>
          </q-card>
          <q-card flat bordered class="my-card q-ma-lg">
            <img src="~assets/croissant.jpg" alt="" />

            <q-card-section>
              <div class="text-h6">Круассан классический</div>
              <div class="text-subtitle2">Мука пшеничная в/с, глютен, инвертный сахар, соль, сахар, дрожжи, молоко 3.2%, масло сливочное.</div>
            </q-card-section>
          </q-card>
          <q-card flat bordered class="my-card q-ma-lg">
            <img src="~assets/cookie.jpg" alt="" />

            <q-card-section>
              <div class="text-h6">Card </div>
              <div class="text-subtitle2">by John Doe</div>
            </q-card-section>
          </q-card>
          <q-card flat bordered class="my-card q-ma-lg">
            <img src="~assets/bread2.jpg" alt="" />

            <q-card-section>
              <div class="text-h6">Card </div>
              <div class="text-subtitle2">by John Doe</div>
            </q-card-section>
          </q-card>
          <q-card flat bordered class="my-card q-ma-lg">
            <img src="~assets/bread2.jpg" alt="" />

            <q-card-section>
              <div class="text-h6">Card </div>
              <div class="text-subtitle2">by John Doe</div>
            </q-card-section>
          </q-card>
        </div>
      </div>
    </q-page-container>
</template>

<script setup>
defineOptions({
  name: 'ProductsPage'
});
</script>
<style lang="sass" scoped>
.my-card
  width: 100%
  max-width: 250px
img
  height: 240px
  width: 250px
</style>
