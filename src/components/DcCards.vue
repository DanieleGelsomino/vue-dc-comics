<template>
  <div class="card">
    <img :src="comics.thumb" :alt="comics.series" />
    <h3>{{ comics.series }}</h3>
  </div>
</template>

<script>
export default {
  name: "DcCards",
  props: {
    comics: Object,
  },
};
</script>

<style scoped lang="scss">
.card {
  border: 2px solid gray;
}
</style>