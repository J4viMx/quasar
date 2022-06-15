<template>
  <q-page class="q-pa-md">
    <span class="text-h3">Dialogs</span>
    <q-separator />

    <div class="q-pa-md q-gutter-sm">
      <q-btn label="Alert" color="primary" @click="alert = true" />
      <q-btn label="Confirm" color="primary" @click="confirm = true" />
      <q-btn label="Prompt" color="primary" @click="prompt = true" />
    </div>

    <q-dialog v-model="alert">
      <q-card>
        <q-card-section>
          <div class="text-h6">Alert</div>
        </q-card-section>

        <q-card-section class="q-pt-none">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Rerum
          repellendus sit voluptate voluptas eveniet porro. Rerum blanditiis
          perferendis totam, ea at omnis vel numquam exercitationem aut, natus
          minima, porro labore.
        </q-card-section>

        <q-card-actions align="right">
          <q-btn flat label="OK" color="primary" v-close-popup />
        </q-card-actions>
      </q-card>
    </q-dialog>
  </q-page>
</template>

<script>
/* import {useQuasar} from 'quasar' */

import { defineComponent } from "vue";
import { ref } from "vue";

export default defineComponent({
  name: "DialogsPage",

  setup() {
    return {
      alert: ref(false),
      confirm: ref(false),
      prompt: ref(false),

      address: ref(""),
    };
  },
});
</script>
