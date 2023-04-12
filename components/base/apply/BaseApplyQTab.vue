<template>
  <div class="q-pa-md">
    <div style="max-width: 100%">
      <q-tabs v-model="tab" align="justify" narrow-indicator class="q-mb-lg">
        <q-tab
          v-for="item in tabs"
          :key="item.name"
          :class="item.color"
          :name="item.name"
          :label="item.label"
        />
      </q-tabs>

      <div class="q-gutter-y-sm">
        <q-tab-panels
          v-for="item in tabs"
          :key="item.name"
          v-model="tab"
          animated
          :transition-prev="item.transitionPrev"
          :transition-next="item.transitionNext"
          :class="item.color + ' text-white text-center'"
        >
          <q-tab-panel
            v-for="panel in item.panels"
            :key="panel.name"
            :name="panel.name"
          >
            <div class="text-h6">{{ panel.label }}</div>
            {{ panel.content }}
          </q-tab-panel>
        </q-tab-panels>
      </div>
    </div>
  </div>
</template>
<script>
import { ref } from "vue";

export default {
  setup() {
    const tab = ref("mails");
    const tabs = [
      {
        name: "mails",
        label: "Mails",
        color: "text-purple",
        transitionPrev: "scale",
        transitionNext: "scale",
        panels: [
          {
            name: "mails",
            label: "Mails",
            content: "Lorem ipsum dolor sit amet consectetur adipisicing elit.",
          },
          {
            name: "alarms",
            label: "Alarms",
            content:
              "Ad molestiae non facere animi nobis, similique nemo velit.",
          },
          {
            name: "movies",
            label: "Movies",
            content: "Nostrum necessitatibus expedita dolores? Voluptatem.",
          },
        ],
      },
      {
        name: "alarms",
        label: "Alarms",
        color: "text-orange",
        transitionPrev: "fade",
        transitionNext: "fade",
        panels: [
          {
            name: "mails",
            label: "Mails",
            content: "Lorem ipsum dolor sit amet consectetur adipisicing elit.",
          },

          {
            name: "alarms",
            label: "Alarms",
            content: "Ad molestiae non facere animi nobis, similique nemo.",
          },
          {
            name: "movies",
            label: "Movies",
            content: "Nostrum necessitatibus expedita dolores? Voluptatem.",
          },
        ],
      },
      {
        name: "movies",
        label: "Movies",
        color: "text-teal",
        transitionPrev: "jump-up",
        transitionNext: "jump-down",
        panels: [
          {
            name: "mails",
            label: "Mails",
            content: "Lorem ipsum dolor sit amet consectetur adipisicing elit.",
          },
          {
            name: "alarms",
            label: "Alarms",
            content: "Ad molestiae non facere animi nobis, similique nemo.",
          },
          {
            name: "movies",
            label: "Movies",
            content: "Nostrum necessitatibus expedita dolores? Voluptatem.",
          },
        ],
      },
      {
        name: "mails",
        label: "Mails",
        color: "text-blue",
        transitionPrev: "scale",
        transitionNext: "scale",
        panels: [
          {
            name: "mails",
            label: "Mails",
            content: "Lorem ipsum dolor sit amet consectetur adipisicing elit.",
          },

          {
            name: "alarms",
            label: "Alarms",
            content:
              "Ad molestiae non facere animi nobis, similique nemo velit.",
          },
          {
            name: "movies",
            label: "Movies",
            content: "Nostrum necessitatibus expedita dolores? Voluptatem.",
          },
        ],
      },
      {
        name: "mails",
        label: "Mails",
        color: "text-pink",
        transitionPrev: "scale",
        transitionNext: "scale",
        panels: [
          {
            name: "mails",
            label: "Mails",
            content: "Lorem ipsum dolor sit amet consectetur adipisicing elit.",
          },
          {
            name: "alarms",
            label: "Alarms",
            content:
              "Ad molestiae non facere animi nobis, similique nemo velit.",
          },
          {
            name: "movies",
            label: "Movies",
            content: "Nostrum necessitatibus expedita dolores? Voluptatem.",
          },
        ],
      },
    ];
    return { tab, tabs };
  },
};
</script>
