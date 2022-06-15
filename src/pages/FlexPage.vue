<template>
  <q-page>
    <div class="row q-mb-md">
      <div class="col bg-primary"></div>
      <div class="col bg-secondary"></div>
      <div class="col bg-accent"></div>
    </div>

    <div class="row q-mb-md">
      <div class="col bg-primary"></div>
      <div class="col-5 bg-secondary"></div>
      <div class="col-6 bg-accent"></div>
    </div>
    <div class="row q-mb-md justify-center">
      <div class="col-4 bg-primary"></div>
      <div class="col-4 bg-secondary"></div>
    </div>

    <q-separator spaced />

    <div class="row q-mb-md">
      <div class="col-12 col-md-6 bg-primary"></div>
      <div class="col-12 col-md-6 bg-secondary"></div>
    </div>

    <q-separator spaced />

    <div class="row q-mb-md">
      <div class="square-box q-mx-md bg-primary"></div>
      <div class="square-box q-mx-md bg-secondary"></div>
      <div class="square-box q-mx-md bg-accent"></div>
    </div>
    <div class="row q-mb-md justify-between">
      <div class="square-box q-mx-md bg-primary"></div>
      <div class="square-box q-mx-md bg-secondary"></div>
      <div class="square-box q-mx-md bg-accent"></div>
    </div>
  </q-page>
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "FlexPage",
});
</script>

<style scoped>
.col,
.col-4,
.col-6,
.col-12 {
  height: 50px;
}

.square-box {
  width: 50px;
  height: 50px;
}
</style>
