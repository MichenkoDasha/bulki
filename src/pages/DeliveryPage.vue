<template>
  <q-page-container>
    <div class="q-pa-md">
      <div class="row justify-center q-gutter-md">

        <q-card
          flat
          bordered
          class="my-card q-ma-lg"
          v-for="p in products"
          v-bind:key="p.img"
        >
          <img :src="'public/products/' + p.img" alt="" />

          <q-card-section>
            <div class="text-h6">{{ p.title }}</div>
            <div class="text-subtitle2">
              {{ p.descr }}
            </div>
          </q-card-section>
        </q-card>

      </div>
    </div>
  </q-page-container>
</template>

<script setup>
import {ref} from "vue";

defineOptions({
  name: 'DeliveryPage'
});

const products = ref([
  {
    "img": "bread1.jpg",
    "title": "Хлеб пшеничный",
    "descr": "Мука пшеничная в/с, мука пшеничная ц/з, вода, соль, мука рисовая."
  },
  {
    "img": "bread3.jpg",
    "title": "Горчичный хлеб",
    "descr": "Пшеничная мука ц/з, Пшеничная мука, соль, сахар, горчичный порошок, вода, дрожжи свежие. дрожжи домашние."
  },
  {
    "img": "bread2.jpg",
    "title": "Багет хрустящий",
    "descr": "Мука пшеничная в/с, вода питьевая, соль, дрожжи хлебопекарные прессованные, мука рисовая."
  },
  {
    "img": "bread4.jpg",
    "title": "Чесночный багет",
    "descr": "Мука пшеничная, дрожжи, вода, соль, сливочное масло, зелень, чеснок, соль, твердый сыр."
  },
  {
    "img": "croissant.jpg",
    "title": "Круассан классический",
    "descr": "Мука пшеничная в/с, глютен, инвертный сахар, соль, сахар, дрожжи, молоко 3.2%, масло сливочное."
  },
  {
    "img": "croissant2.jpg",
    "title": "Круассан с марципаном",
    "descr": "Пшеничная мука, сливочное масло, вода, сахар, сухие дрожжи, соль, очищенный миндаль, ванильный экстракт."
  },
  {
    "img": "cookie.jpg",
    "title": "Печенье мультизлаковое",
    "descr": "Цельные хлопья овса, тростниковый сахар, масло сливочное 82%, цукаты, изюм, тыквенные семечки, яйца, мука пшеничная  в/с, разрыхлитель, соль."
  },
  {
    "img": "eclair.jpg",
    "title": "Ванильный эклер",
    "descr": "Мука пшеничная в/с, мука ц/з, масло сливочное 82%, сливки 33%,  молоко, яйца, сахар, глюкоза, крахмал кукурузный, молочный  шоколад, гель нейтральный, желатин, соль морская."
  },
])

</script>

<style lang="sass" scoped>
.my-card
  width: 100%
  max-width: 260px

img
  height: 240px
  width: 260px

</style>
