<template>
  <q-layout view="lHh Lpr lFf">

    <q-header elevated>
      <q-toolbar class="q-toolbar">
<!--        <q-btn-->
<!--          flat-->
<!--          dense-->
<!--          round-->
<!--          icon="menu"-->
<!--          aria-label="Menu"-->
<!--          @click="toggleLeftDrawer"-->
<!--        />-->

        <q-toolbar-title style="padding: 0px 200px">
          Булки.Онлайн
        </q-toolbar-title>

        <div class="q-pa-md q-gutter-sm">
          <q-breadcrumbs active-color="" style="font-size: 20px">
            <q-breadcrumbs-el label="О нас" to="/start/pick-quasar-flavour" />


            <q-breadcrumbs-el color="primary" label="Продукция">
              <q-menu
                transition-show="scale"
                transition-hide="scale"
              >
                <q-list style="min-width: 100px">
                  <q-item clickable>
                    <q-item-section>Хлеб</q-item-section>
                  </q-item>
                  <q-item clickable>
                    <q-item-section>Пироги</q-item-section>
                  </q-item>
                  <q-separator />
                  <q-item clickable>
                    <q-item-section>Выпечка</q-item-section>
                  </q-item>
                  <q-item clickable>
                    <q-item-section>Печенье</q-item-section>
                  </q-item>
                </q-list>
              </q-menu>
            </q-breadcrumbs-el>
            <q-breadcrumbs-el label="Доставка" to="/vue-components/breadcrumbs" />
            <q-breadcrumbs-el label="Написать нам" to="/vue-components/breadcrumbs" />
          </q-breadcrumbs>
        </div>
<!--        <div class="q-pa-md q-gutter-sm">-->
<!--          <q-btn align="around" outline style="color: goldenrod;" label="Корзина" icon="shopping_cart" />-->
<!--        </div>-->
      </q-toolbar>
    </q-header>
<!--    <q-page-container>-->
      <router-view />

      <q-card class="my-card">
        <q-card-section horizontal>
          <q-img
            class="col-5"
            src="~assets/shop.jpg"/>

          <q-card-section style="font-size: 20px">
            <div class="About"><h3>О нас</h3>
              <p>«Булки.Онлайн» — это пекарня с вкусной, недорогой и свежей продукцией. Мы даём людям возможность заказать свежеиспечённый хлеб, кондитерские изделия, сладкую и сытную выпечку в пекарне. ОНЛАЙН!</p>
            <p> «Булки.Онлайн» — это место, где покупатели могут приобрести свежий вкусный хлеб и выпечку по привлекательным ценам онлайн с доставкой к вашему дому!</p>
            Также мы предлагаем записаться на мактер-класс по выпечке!
              <p>В течение мастер-класса вы отработаете навыки приготовления хрустящего хлеба, а также рецепты по приготовлению вкуснейшей выпечки от начала и до конца, так что в дальнейшем вы сможете с лёгкостью применить эти навыки дома.</p>
              <h3>Что мы предлагаем:</h3>
              <li>
                Занятия в стильной студии с современным кухонным оборудованием
              </li>
              <li>
                4 часа кулинарной практики под руководством опытного наставника
              </li>
              <li>
                Индивидуальное рабочее место и набор продуктов
              </li>
              <li>
                Подробные технологические карты всех блюд
              </li>
            </div>
          </q-card-section>
        </q-card-section>


      </q-card>
<!--    <q-separator />-->
    <q-footer elevated>
      <q-toolbar>
        <q-toolbar-title>
          <q-breadcrumbs active-color="" gutter="lg">
            <q-breadcrumbs-el label="Рабочие дни: ПН-ВС" />
            <q-breadcrumbs-el label="Время работы: 7:30 - 20:30" />
            <q-btn label="Записаться" style="font-size: 20px">
            </q-btn>
<!--            <q-btn outline label="Записаться" icon="question_answer"/>-->
          </q-breadcrumbs>

        </q-toolbar-title>
      </q-toolbar>
    </q-footer>
<!--            <div class="q-footer">-->
<!--              <div class="container">-->
<!--              <q-btn flat round icon="event" />-->
<!--              <q-btn flat>-->
<!--                Рабочие дни: ПН-ВС-->
<!--              </q-btn>-->
<!--              <q-btn flat>-->
<!--                Время работы: 7:30 - 20:30-->
<!--              </q-btn>-->
<!--              <q-btn flat color="primary">-->
<!--                Написать нам-->
<!--              </q-btn>-->
<!--              </div>-->
<!--            </div>-->

<!--    </q-page-container>-->
<!--    <q-drawer-->
<!--      v-model="leftDrawerOpen"-->
<!--      show-if-above-->
<!--      bordered-->
<!--    >-->
<!--      <q-list>-->
<!--        <q-item-label-->
<!--          header-->
<!--        >-->
<!--          Essential Links-->
<!--        </q-item-label>-->

<!--        <EssentialLink-->
<!--          v-for="link in linksList"-->
<!--          :key="link.title"-->
<!--          v-bind="link"-->
<!--        />-->
<!--      </q-list>-->
<!--    </q-drawer>-->


  </q-layout>
</template>

<script setup>

// import { ref } from 'vue'
// import EssentialLink from 'components/EssentialLink.vue'

defineOptions({
  name: 'MainLayout'
})
//
// const linksList = [
//   {
//     title: 'Docs',
//     caption: 'quasar.dev',
//     icon: 'school',
//     link: 'https://quasar.dev'
//   },
//   {
//     title: 'Github',
//     caption: 'github.com/quasarframework',
//     icon: 'code',
//     link: 'https://github.com/quasarframework'
//   },
//   {
//     title: 'Discord Chat Channel',
//     caption: 'chat.quasar.dev',
//     icon: 'chat',
//     link: 'https://chat.quasar.dev'
//   },
//   {
//     title: 'Forum',
//     caption: 'forum.quasar.dev',
//     icon: 'record_voice_over',
//     link: 'https://forum.quasar.dev'
//   },
//   {
//     title: 'Twitter',
//     caption: '@quasarframework',
//     icon: 'rss_feed',
//     link: 'https://twitter.quasar.dev'
//   },
//   {
//     title: 'Facebook',
//     caption: '@QuasarFramework',
//     icon: 'public',
//     link: 'https://facebook.quasar.dev'
//   },
//   {
//     title: 'Quasar Awesome',
//     caption: 'Community Quasar projects',
//     icon: 'favorite',
//     link: 'https://awesome.quasar.dev'
//   }
// ]

// const leftDrawerOpen = ref(false)

// function toggleLeftDrawer () {
//   leftDrawerOpen.value = !leftDrawerOpen.value
// }
</script>
<style lang="sass" scoped>
.my-card
  width: 100%
  max-width: 1500px
  margin: 10px auto 20px
  display: block
.q-toolbar
  color: #BD944C


</style>
