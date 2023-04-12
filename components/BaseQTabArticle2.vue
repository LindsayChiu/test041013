<!-- <template>
  <div class="q-pa-md">
    <div style="max-width: 100%">
      <q-tabs v-model="tab" align="justify" narrow-indicator class="q-mb-lg">
        <q-tab name="mails" label="Mails" />
        <q-tab name="alarms" label="Alarms" />
        <q-tab name="movies" label="Movies" />
      </q-tabs>

      <div class="q-gutter-y-sm">
        <q-tab-panels v-model="tab">
          <q-tab-panel name="mails">
            <div class="text-h6">Mails</div>
            111Lorem ipsum dolor sit amet consectetur adipisicing elit.
          </q-tab-panel>
        </q-tab-panels>

        <q-tab-panels v-model="tab">
          <q-tab-panel name="mails">
            <div class="text-h6">Mails</div>
            222Lorem ipsum dolor sit amet consectetur adipisicing elit.
          </q-tab-panel>

          <q-tab-panel name="alarms">
            <div class="text-h6">Alarms</div>
            222Ad molestiae non facere animi nobis, similique nemo.
          </q-tab-panel>

          <q-tab-panel name="movies">
            <div class="text-h6">Movies</div>
            222Nostrum necessitatibus expedita dolores? Voluptatem.
          </q-tab-panel>
        </q-tab-panels>

        <q-tab-panels v-model="tab">
          <q-tab-panel name="mails">
            <div class="text-h6">Mails</div>
            333Lorem ipsum dolor sit amet consectetur adipisicing elit.
          </q-tab-panel>

          <q-tab-panel name="alarms">
            <div class="text-h6">Alarms</div>
            333Ad molestiae non facere animi nobis, similique nemo.
          </q-tab-panel>

          <q-tab-panel name="movies">
            <div class="text-h6">Movies</div>
            333Nostrum necessitatibus expedita dolores? Voluptatem.
          </q-tab-panel>
        </q-tab-panels>

        <q-tab-panels v-model="tab">
          <q-tab-panel name="mails">
            <div class="text-h6">Mails</div>
            111Lorem ipsum dolor sit amet consectetur adipisicing elit.
          </q-tab-panel>

          <q-tab-panel name="alarms">
            <div class="text-h6">Alarms</div>
            111Ad molestiae non facere animi nobis, similique nemo velit.
          </q-tab-panel>

          <q-tab-panel name="movies">
            <div class="text-h6">Movies</div>
            111Nostrum necessitatibus expedita dolores? Voluptatem.
          </q-tab-panel>
        </q-tab-panels>

        <q-tab-panels v-model="tab">
          <q-tab-panel name="mails">
            <div class="text-h6">Mails</div>
            222Lorem ipsum dolor sit amet consectetur adipisicing elit.
          </q-tab-panel>

          <q-tab-panel name="alarms">
            <div class="text-h6">Alarms</div>
            222Ad molestiae non facere animi nobis, similique nemo.
          </q-tab-panel>

          <q-tab-panel name="movies">
            <div class="text-h6">Movies</div>
            222Nostrum necessitatibus expedita dolores? Voluptatem.
          </q-tab-panel>
        </q-tab-panels>

        <q-tab-panels v-model="tab">
          <q-tab-panel name="mails">
            <div class="text-h6">Mails</div>
            555Lorem ipsum dolor sit amet consectetur adipisicing elit.
          </q-tab-panel>

          <q-tab-panel name="alarms">
            <div class="text-h6">Alarms</div>
            555Ad molestiae non facere animi nobis, similique nemo velit.
          </q-tab-panel>

          <q-tab-panel name="movies">
            <div class="text-h6">Movies</div>
            555Nostrum necessitatibus expedita dolores? Voluptatem.
          </q-tab-panel>
        </q-tab-panels>

        <q-tab-panels v-model="tab">
          <q-tab-panel name="mails">
            <div class="text-h6">Mails</div>
            666Lorem ipsum dolor sit amet consectetur adipisicing elit.
          </q-tab-panel>

          <q-tab-panel name="alarms">
            <div class="text-h6">Alarms</div>
            666Ad molestiae non facere animi nobis, similique nemo.
          </q-tab-panel>

          <q-tab-panel name="movies">
            <div class="text-h6">Movies</div>
            666Nostrum necessitatibus expedita dolores? Voluptatem.
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

<!-- <template>
  <div class="q-pa-md">
    <div style="max-width: 100%">
      <q-tabs v-model="tab" align="justify" narrow-indicator class="q-mb-lg">
        <q-tab
          v-for="item in items"
          :key="item.name"
          :name="item.name"
          :label="item.label"
        />
      </q-tabs>

      <div class="q-gutter-y-sm">
        <q-tab-panels v-model="tab">
          <q-tab-panel v-for="item in items" :key="item.name" :name="item.name">
            <div class="text-h6">{{ item.label }}</div>
            {{ item.content }}
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
    const items = [
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
      {
        name: "movies1",
        label: "Movies1",
        content: "111Nostrum necessitatibus expedita dolores? Voluptatem.",
      },
    ];
    return {
      tab,
      items,
    };
  },
};
</script> -->

<template>
  <div class="q-pa-md">
    <div style="max-width: 100%">
      <q-tabs v-model="tab" align="justify" narrow-indicator class="q-mb-lg">
        <q-tab
          v-for="item in items"
          :key="item.name"
          :name="item.name"
          :label="item.label"
        />
      </q-tabs>

      <div class="q-gutter-y-sm">
        <q-tab-panels v-model="tab">
          <q-tab-panel v-for="item in items" :key="item.name" :name="item.name">
            <component :is="item.content" />
          </q-tab-panel>
        </q-tab-panels>
      </div>
    </div>
  </div>
</template>

<script>
import { ref } from "vue";
import BaseAtcList from "~/components/base/apply/BaseAtcList.vue";

export default {
  components: {
    BaseAtcList,
  },
  setup() {
    const tab = ref("mails");
    const items = [
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
      {
        name: "movies1",
        label: "Movies1",
        content: "111Nostrum necessitatibus expedita dolores? Voluptatem.",
      },
      {
        name: "BaseAtcList",
        label: "My Card List",
        content: BaseAtcList,
      },
    ];
    return {
      tab,
      items,
    };
  },
};
</script>
