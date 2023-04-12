<template>
  <div>
    <my-card
      v-for="item in items"
      :key="item.id"
      :title="item.title"
      :content="item.content"
      :img="item.img"
    />
  </div>
</template>

<script>
import BaseApplyAtc from "./BaseApplyAtc.vue";

export default {
  components: {
    BaseApplyAtc,
  },
  setup() {
    const items = [
      {
        id: 1,
        title: "文章標題1",
        content:
          "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.",
        img: "https://cdn.quasar.dev/img/parallax2.jpg",
      },
      {
        id: 2,
        title: "文章標題2",
        content:
          "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.",
        img: "https://cdn.quasar.dev/img/parallax2.jpg",
      },
      {
        id: 3,
        title: "文章標題3",
        content:
          "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.",
        img: "https://cdn.quasar.dev/img/parallax2.jpg",
      },
    ];

    return {
      items,
    };
  },
};
</script>
