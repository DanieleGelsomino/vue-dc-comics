<template>
  <div class="card">
    <img :src="urlImg" />
    <h3>{{ titleSeries }}</h3>
  </div>
</template>

<script>
export default {
  name: "DcCards",
  props: {
    urlImg: String,
    titleSeries: String,
  },
};
</script>

<style scoped lang="scss">
@import "@/variables";
.card {
  display: $d-flex;
  width: calc(100% / 6);
  flex-direction: column;
  flex-wrap: wrap;

  img {
    width: 100px;
    height: 100px;
  }

  h3 {
    color: $text-white;
    font-size: $font-size-6;
    text-align: left;
    line-height: 10px;
  }
}
</style>