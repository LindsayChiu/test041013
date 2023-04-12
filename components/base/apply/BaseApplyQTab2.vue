<!-- <template>
  <div class="q-pa-md">
    <div style="max-width: 100%">
      <q-tabs v-model="tab" align="justify" narrow-indicator class="q-mb-lg">
        <q-tab class="text-purple" name="mails" label="Mails" />
      </q-tabs>

      <div class="q-gutter-y-sm">
        <q-tab-panels
          v-model="tab"
          animated
          transition-prev="scale"
          transition-next="scale"
          class="bg-purple text-white text-center"
        >
          <q-tab-panel name="mails">
            <div class="text-h6">Mails</div>
            111Lorem ipsum dolor sit amet consectetur adipisicing elit.
          </q-tab-panel>
        </q-tab-panels>

        <q-tab-panels
          v-model="tab"
          animated
          transition-prev="fade"
          transition-next="fade"
          class="bg-orange text-white text-center"
        >
          <q-tab-panel name="mails">
            <div class="text-h6">Mails</div>
            333Lorem ipsum dolor sit amet consectetur adipisicing elit.
          </q-tab-panel>
        </q-tab-panels>

        <q-tab-panels
          v-model="tab"
          animated
          transition-prev="jump-up"
          transition-next="jump-down"
          class="bg-teal text-white text-center"
        >
          <q-tab-panel name="mails">
            <div class="text-h6">Mails</div>
            444Lorem ipsum dolor sit amet consectetur adipisicing elit.
          </q-tab-panel>
        </q-tab-panels>

        <q-tab-panels
          v-model="tab"
          animated
          transition-prev="scale"
          transition-next="scale"
          class="bg-purple text-white text-center"
        >
          <q-tab-panel name="mails">
            <div class="text-h6">Mails</div>
            555Lorem ipsum dolor sit amet consectetur adipisicing elit.
          </q-tab-panel>
        </q-tab-panels>

        <q-tab-panels
          v-model="tab"
          animated
          transition-prev="fade"
          transition-next="fade"
          class="bg-orange text-white text-center"
        >
          <q-tab-panel name="mails">
            <div class="text-h6">Mails</div>
            666Lorem ipsum dolor sit amet consectetur adipisicing elit.
          </q-tab-panel>
        </q-tab-panels>
        <q-tab-panels
          v-model="tab"
          animated
          transition-prev="scale"
          transition-next="scale"
          class="bg-purple text-white text-center"
        >
          <q-tab-panel name="mails">
            <div class="text-h6">Mails</div>
            777Lorem ipsum dolor sit amet consectetur adipisicing elit.
          </q-tab-panel>
        </q-tab-panels>

        <q-tab-panels
          v-model="tab"
          animated
          transition-prev="fade"
          transition-next="fade"
          class="bg-orange text-white text-center"
        >
          <q-tab-panel name="mails">
            <div class="text-h6">Mails</div>
            888Lorem ipsum dolor sit amet consectetur adipisicing elit.
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
    return {
      tab: ref("mails"),
    };
  },
};
</script> -->

<template>
  <div class="q-pa-md">
    <div style="max-width: 100%">
      <q-tabs v-model="tab" align="justify" narrow-indicator class="q-mb-lg">
        <q-tab
          v-for="panel in panels"
          :key="panel.name"
          :name="panel.name"
          :label="panel.label"
          :class="panel.color"
        />
      </q-tabs>

      <div class="q-gutter-y-sm">
        <q-tab-panels
          v-for="panel in panels"
          :key="panel.name"
          v-model="tab"
          :animated="true"
          :transition-prev="panel.transitionPrev"
          :transition-next="panel.transitionNext"
          :class="panel.color + ' text-white text-center'"
        >
          <q-tab-panel :name="panel.name">
            <div class="text-h6">{{ panel.label }}</div>
            <p>{{ panel.content }}</p>
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
    const panels = [
      {
        name: "mails",
        label: "Mails",
        color: "text-purple",
        transitionPrev: "scale",
        transitionNext: "scale",
        content: [
          "Lorem ipsum dolor sit amet consectetur adipisicing elit.",
          "Lorem ipsum dolor sit amet consectetur adipisicing elit.",
        ],
      },
      {
        name: "mails",
        label: "Mails",
        color: "text-pink",
        transitionPrev: "scale",
        transitionNext: "scale",
        content: "111Lorem ipsum dolor sit amet consectetur adipisicing elit.",
      },
      {
        name: "alarms",
        label: "Alarms",
        color: "text-orange",
        transitionPrev: "fade",
        transitionNext: "fade",
        content: "Ad molestiae non facere animi nobis, similique nemo.",
      },
      {
        name: "movies",
        label: "Movies",
        color: "text-teal",
        transitionPrev: "jump-up",
        transitionNext: "jump-down",
        content: "Nostrum necessitatibus expedita dolores? Voluptatem.",
      },
    ];

    return {
      tab: ref("mails"),
      panels,
    };
  },
};
</script>
