<template>
  <div class="entry-title d-flex justify-content-between p-2">
    <div class="">
      <span class="text-success fs-3 fw-bold">20</span>
      <span class="mx-1 fs-3">Abril</span>
      <span class="mx-2 fs-4 fw-light">2024, Sabado</span>
    </div>
    <div class="">
      <button class="btn btn-danger mx-2">
        borrar
        <i class="fa fa-trash-alt"></i>
      </button>
      <button class="btn btn-primary">
        Subir Foto
        <i class="fa fa-upload"></i>
      </button>
    </div>
  </div>
  <hr />
  <div class="d-flex flex-column px-3 h-75">
    <textarea placeholder="Que Sucedio Hoy?"> </textarea>
  </div>
  <FabComponent icon="fa-save" />
  <img
    class="img-thumbnail"
    src="https://i.pinimg.com/originals/6d/58/9c/6d589cd23e8857fb50465aa557e5bd3f.jpg"
    alt="Robert"
  />
</template>

<script>
import { defineAsyncComponent } from "vue";

export default {
  name: "EntryView",
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
.img-thumbnail {
    width: 200px;
    position: fixed;
    bottom: 150px;
    right: 20px;
    box-shadow: 0px 5px 10px rgba($color:#000, $alpha:0.2);
}
textarea {
  height: 100%;
  border: none;
  font-size: 20px;

  &:focus {
    outline: none;
  }
}
</style>
