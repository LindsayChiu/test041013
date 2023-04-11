<template>
  <q-input
    color="grey-3"
    label-color="orange"
    outlined
    v-model="text"
    label="Search..."
  >
    <template v-slot:append>
      <q-icon :name="matSearch" left size="2em" color="orange" />
    </template>
  </q-input>
</template>

<script>
import { matSearch } from "@quasar/extras/material-icons";

export default {
  setup() {
    return {
      text: ref(""),
    };
  },
};
</script>
