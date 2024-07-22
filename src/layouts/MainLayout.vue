<template>
  <q-layout view="lHh Lpr lFf" class="shrink">
    <q-header elevated class="shrink">
      <q-toolbar class="q-toolbar">
        <q-toolbar-title>
          <q-btn class="text-h6" flat label="Булки.Онлайн" to="/" />
        </q-toolbar-title>
        <q-space />
        <q-btn-group flat>
          <q-btn to="/" label="О нас" />
          <q-btn to="/products" label="Мероприятия" />
          <q-btn to="/delivery" label="Галерея" />
          <q-btn to="/contacts" label="Написать нам" />
        </q-btn-group>
      </q-toolbar>
    </q-header>

    <q-page-container class="shrink">
      <router-view />
    </q-page-container>

    <q-footer elevated class="shrink">
      <q-toolbar>
        <q-toolbar-title>
          Рабочие дни: ПН-ВС / Время работы: 7:30 - 20:30
        </q-toolbar-title>
        <q-btn flat label="Записаться" />
      </q-toolbar>
    </q-footer>
  </q-layout>
</template>

<script setup>

defineOptions({
  name: 'MainLayout',
})
</script>

<style lang="sass" scoped>
.q-toolbar
  color: #BD944C

.shrink
  max-width: 1500px
  margin: auto
</style>
