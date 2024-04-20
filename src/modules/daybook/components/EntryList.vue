<template>
  <div class="entry-list-container">
    <div class="px-2 pt-2">
      <input type="text" class="form-control" placeholder="Buscar Entrada" />
    </div>
    <div class="entry-scrollarea">
      
        <entry-component v-for="item in 100" :key="item"/>
      
    </div>
  </div>
</template>

<script>
import { defineAsyncComponent } from "vue";

export default {
  components: { 
    EntryComponent: defineAsyncComponent(() => import(/* webpackChunkName: "daybook-entry" */ './EntryComponent.vue'))
     },};
</script>

<style lang="scss" scoped>
input{
    margin-bottom: 8px;
}

.entry-list-container{
    border-right: 1px solid #2c3e50;
    height: calc(100vh - 56px);
}

.entry-scrollarea{
    overflow-y: auto;
    height: calc(100vh - 110px);
}


</style>
