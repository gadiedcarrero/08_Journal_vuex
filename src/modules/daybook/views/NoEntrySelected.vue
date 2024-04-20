<template>
  <div class="d-flex justify-content-center">
    <h1 class="align-self-center">No Entry selected</h1>
    
  </div>
  <fab-component />
</template>

<script>
import { defineAsyncComponent } from "vue";
export default {
  name: "NoEntrySelected",
  components: {
    FabComponent: defineAsyncComponent(() =>
      import(
        /* webpackChunkName: "fab-component" */ "../components/FabComponent.vue"
      )
    ),
  },
};
</script>

<style lang="scss" scoped>
div {
  height: 100%;
}
</style>
