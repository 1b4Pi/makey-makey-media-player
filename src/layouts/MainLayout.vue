<template>
  <q-layout view="hHh lpR fFf" style="background: #000">
    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "MainLayout",

  setup() {},
});
</script>
