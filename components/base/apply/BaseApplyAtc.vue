<!-- <template>
  <div class="q-pa-md row items-start q-gutter-md">
    <q-card class="my-card" flat bordered>
      <q-card-section horizontal>
        <q-img class="col-3" :src="img" />
        <q-card-section>
          <div class="text-h5 q-mt-sm q-mb-xs">{{ title }}</div>
          <div class="text-caption text-grey">
            {{ lorem }}
          </div>
        </q-card-section>
      </q-card-section>
    </q-card>
  </div>
</template>

<script>
export default {
  setup() {
    return {
      title: "文章標題",
      lorem:
        "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.",
      img: "https://cdn.quasar.dev/img/parallax2.jpg",
    };
  },
};
</script> -->

<template>
  <div class="q-pa-md row items-start q-gutter-md">
    <q-card class="my-card" flat bordered>
      <q-card-section horizontal>
        <q-img class="col-3" :src="img" />
        <q-card-section>
          <div class="text-h5 q-mt-sm q-mb-xs">{{ title }}</div>
          <div class="text-caption text-grey">
            {{ content }}
          </div>
        </q-card-section>
      </q-card-section>
    </q-card>
  </div>
</template>

<script>
export default {
  props: {
    title: {
      type: String,
      default: "",
    },
    content: {
      type: String,
      default: "",
    },
    img: {
      type: String,
      default: "https://cdn.quasar.dev/img/parallax2.jpg",
    },
  },
};
</script>
