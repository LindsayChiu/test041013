<template>
  <q-layout view="hHh lpR fff">
    <q-header class="bg-white text-primary" height-hint="98">
      <BaseApplyLogin />
      <q-toolbar>
        <q-toolbar-title class="bg-white text-primary">
          <q-avatar>
            <img src="https://cdn.quasar.dev/logo-v2/svg/logo-mono-white.svg" />
          </q-avatar>
          心閱網
        </q-toolbar-title>
        <BaseApplySearch />
      </q-toolbar>

      <q-tabs align="center">
        <q-route-tab to="/page1" label="所有文章" />
        <q-route-tab to="/page2" label="智慧小語" />
        <q-route-tab to="/page3" label="出版專區" />
        <q-route-tab to="/page4" label="活動專區" />
        <q-route-tab to="/page5" label="影音專區" />
      </q-tabs>
    </q-header>

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script setup></script>
