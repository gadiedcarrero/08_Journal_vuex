<template>
  <button class="btn btn-primary">
    <i :class="['fa fa-2x', icon]"></i>
  </button>
</template>

<script>
export default {
  name: 'FabComponent',
  props:{
    icon:{
      type: String,
      default: 'fa-plus'
    }
  }
  
};

</script>

<style lang="scss" scoped>
i{
  font-size: 18px;
}
button {
  position: fixed;
  bottom: 20px;
  right: 20px;
  border-radius: 50%;
  width: 40px;
  height: 40px;
  display: inline-flex;
  justify-content: center;
  align-items: center;
}

</style>