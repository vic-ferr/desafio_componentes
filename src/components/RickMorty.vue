<template>
  <div class="box-general">
    <div class="col-12 box-rick-and-morty">
      <img
        :src="animex.image"
        :alt="animex.name"
        width="100"
        height="100"
        class="imagen-rick"
      />
      <h3 class="box-name-h3">{{ animex.name }}</h3>
    </div>
  </div>
</template>

<script>
export default {
  name: "RickMorty",
  props: {
    animex: {
      type: Object,
      default: () => {},
    },
  },
};
</script>
