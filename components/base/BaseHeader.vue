<template>
  <q-layout view="hHh lpR fff">
    <q-header class="bg-primary text-white" height-hint="98">
      <BaseApplySearch />
      <q-toolbar>
        <q-toolbar-title>
          <q-avatar>
            <img src="https://cdn.quasar.dev/logo-v2/svg/logo-mono-white.svg" />
          </q-avatar>
          Title
        </q-toolbar-title>
        <BaseApplyLogin />
      </q-toolbar>

      <q-tabs align="center">
        <q-route-tab to="/page1" label="Page One" />
        <q-route-tab to="/page2" label="Page Two" />
        <q-route-tab to="/page3" label="Page Three" />
        <q-route-tab to="/page4" label="Page Four" />
        <q-route-tab to="/page5" label="Page Five" />
      </q-tabs>
    </q-header>

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script setup></script>
