<template>
    <q-page-container>
      <div class="q-pa-md">
        <div class="row justify-center q-gutter-md">
            <q-card
              flat
              bordered
              class="my-card q-ma-lg"
              v-for="p in products"
              :key="p.title"
            >
              <img :src="'products/' + p.img" alt="" />
              <q-card-section>
                <div class="text-h6">{{ p.title }}</div>
                <div class="text-subtitle2">
                  {{ p.decr }}
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
  name: 'ProductsPage'
});

const products = ref([
  {
    img: 'bread1.jpg',
    title: 'Хлеб пшеничный',
    decr: 'Мука пшеничная в/с, мука пшеничная ц/з, вода, соль, мука рисовая.'
  },
  {
    img: 'bread2.jpg',
    title: 'Багет хрустящий',
    decr: 'Мука пшеничная в/с, вода питьевая, соль, дрожжи хлебопекарные прессованные, мука рисовая.'
  },
  {
    img: 'croissant.jpg',
    title: 'Круассан классический',
    decr: 'Мука пшеничная в/с, глютен, инвертный сахар, соль, сахар, дрожжи, молоко 3.2%, масло сливочное.'
  },
  {
    img: 'cookie.jpg',
    title: 'Хлеб пшеничный',
    decr: 'Мука пшеничная в/с, мука пшеничная ц/з, вода, соль, мука рисовая.'
  }
])

</script>

<style lang="sass" scoped>
.my-card
  width: 100%
  max-width: 250px
img
  height: 240px
  width: 250px
</style>
