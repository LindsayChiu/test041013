<template>
  <div class="q-pa-md">
    <div class="q-gutter-md" style="max-width: 300px">
      <q-input rounded outlined v-model="text" label="Rounded outlined" />
    </div>
  </div>
</template>

<script>
export default {
  setup() {
    return {
      text: ref(""),
    };
  },
};
</script>
