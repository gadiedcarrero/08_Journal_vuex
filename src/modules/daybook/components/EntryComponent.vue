<template>
  <div @click="$router.push({name:'entry', params:{id:10}})" class="entry-container mb-3 pointer p-2">
    <div class="entry-title d-flex">
      <span class="text-success fs-5 fw-bold">20</span>
      <span class="mx-1 fs-5">Abril</span>
      <span class="mx-2 fw-light">2024, Sabado</span>
    </div>
    <div class="entry-description">
      Irure ipsum laborum anim esse consectetur minim deserunt excepteur. Sint
      eu veniam deserunt eu sit commodo consectetur reprehenderit aute velit
      duis dolore. Ea aliqua voluptate amet sint labore dolor elit proident
      excepteur sunt ut. Laborum veniam id amet commodo elit do ipsum aliqua
      fugiat veniam aute.
    </div>
  </div>
</template>

<script>
export default {
  name: "EntryComponent",
  methods: {
    
  },
};
</script>

<style lang="scss" scoped>

.entry-container {
  border-bottom: 1px solid #2c3e50;
  transition: 0.2s all ease-in;

  &:hover {
    background-color: lighten($color: grey, $amount: 45);
    transition: 0.2s all ease-in;
  }
}
.entry-description{
  font-size: 12px;
}


</style>
