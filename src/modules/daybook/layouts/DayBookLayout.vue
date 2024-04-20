<template>
  <navbar-component/>
  <div class="d-flex">
    <div class="col-4">
      <entry-list/>
    </div>
    <div class="col">
      <router-view/>
    </div>
  </div>
</template>
<script>
import { defineAsyncComponent } from "vue";

export default {
  name: 'DayBookLayout',
  components: {
    NavbarComponent: defineAsyncComponent(() => import(/* webpackChunkName: "daybook-navbar" */ '../components/NavbarComponent.vue')),
    EntryList: defineAsyncComponent(() => import(/* webpackChunkName: "daybook-entry-list" */ '../components/EntryList.vue'))
  }
}
</script>
