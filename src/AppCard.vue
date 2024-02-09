<script>
export default {
  props: {
    img: String,
    title: String,
  },
};
</script>

<template>
  <div class="card">
    <img :src="img" :alt="title" />
    <h3>{{ title }}</h3>
  </div>
</template>

<style lang="scss" scoped>
.card {
  position: relative;
  width: calc((100% / 3) - 20px);
  min-width: 300px;
  border: 1px dashed black;
  margin: 10px;
  min-height: 200px;
}
</style>
