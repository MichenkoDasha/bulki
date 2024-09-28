<template>
  <q-page-container class="q-pa-xs">
    <div class="q-ml-lg text-h5">
      Расписание мероприянтий
    </div>

    <q-separator class="q-ma-lg" />

    <q-list>
      <q-item v-for="c in courses" v-bind:key="c.date" class="q-mb-sm">
        <q-item-section avatar>
          <q-avatar>
            <img :src="`public/courses/${c.img}`" alt="">
          </q-avatar>
        </q-item-section>

        <q-item-section>
          <q-item-label>{{ c.title }}</q-item-label>
          <q-item-label caption lines="1">{{ c.descr }}</q-item-label>
        </q-item-section>

        <q-item-section>
          <q-item-label>дата</q-item-label>
          <q-item-label caption lines="1">{{ c.date }}</q-item-label>
        </q-item-section>

        <q-item-section>
          <q-item-label>мастер</q-item-label>
          <q-item-label caption lines="1">{{ c.master }}</q-item-label>
        </q-item-section>

        <q-item-section side>
          <q-btn flat type="link" class="q-banner" label="записаться" href="https://wa.me/79587629882" />
        </q-item-section>
      </q-item>
    </q-list>
  </q-page-container>
</template>

<script setup>
import {ref} from "vue";

defineOptions({
  name: 'ProductsPage'
});

const courses = ref([
  {
    'img': 'wien.jpg',
    'date': '24 августа',
    'title': 'Венская выпечка',
    'descr': 'практический курс для любого уровня',
    'master': 'Миченко Д. Д.'
  },
  {
    'img': 'bf.jpg',
    'date': '02 сентября',
    'title': 'Завтраки',
    'descr': 'практический курс',
    'master': 'Миченко Д. Д.'
  },
//   ...
])

</script>

<style lang="sass" scoped>
.q-banner
  color: #BD944C
</style>
