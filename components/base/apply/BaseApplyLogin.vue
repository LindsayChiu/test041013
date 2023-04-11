<template>
  <div class="q-pa-md q-gutter-md">
    <a href="#">
      <q-btn color="teal">
        <q-icon left size="3em" :name="matAccountCircle" />
        <div>登入 | 註冊</div>
      </q-btn></a
    >

    <q-btn round>
      <q-avatar size="42px">
        <a href="#"><img src="https://cdn.quasar.dev/img/avatar2.jpg" /></a>
      </q-avatar>
    </q-btn>
    <q-btn round>
      <q-avatar size="42px">
        <a href="#"><img src="https://cdn.quasar.dev/img/avatar2.jpg" /></a>
      </q-avatar>
    </q-btn>

    <q-btn round>
      <q-avatar size="42px">
        <a href="#"><img src="https://cdn.quasar.dev/img/avatar2.jpg" /></a>
      </q-avatar>
    </q-btn>
  </div>
</template>

<script setup>
import { matAccountCircle } from "@quasar/extras/material-icons";
</script>
