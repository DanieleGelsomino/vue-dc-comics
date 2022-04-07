<template>
  <div class="card">
    <div class="img-box">
      <img :src="urlImg" />
    </div>
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
  width: (100% / 6);

  .img-box {
    height: 120px;
    width: 130px;
    overflow: hidden;
    margin: 10px 0px;
    padding: 10px;
    img {
      width: 100%;
    }
  }

  h3 {
    color: $text-white;
    font-size: $font-size-6;
    text-transform: $text-uppercase;
    line-height: 10px;
    text-align: left;
    margin-top: 5px;
    margin-left: 10px;
  }
}
</style>