<template>
  <main>
    <div class="jumbotron jumbo-area">
      <div class="badge-series">current series</div>
    </div>
    <div class="container-cards">
      <Cards
        v-for="(item, index) in comics"
        :key="'comic-' + index"
        :titleSeries="item.series"
        :urlImg="item.thumb"
      />
    </div>
    <div class="button">
      <button class="btn-load">load more</button>
    </div>
  </main>
</template>

<script>
import Cards from "@/components/DcCards.vue";
export default {
  name: "MainComponent",
  props: {
    comics: Array,
  },
  components: {
    Cards,
  },
};
</script>

<style scoped lang="scss">
@import "@/variables";

.jumbotron {
  background-image: url("@/assets/jumbotron.jpg");
  background-position: top;
  background-size: 100%;
  background-repeat: no-repeat;
  width: 100%;
}
.jumbo-area {
  height: 300px;
  position: relative;

  .badge-series {
    color: $text-white;
    font-size: $font-size-7;
    background-color: $text-azure;
    font-weight: $text-bold;
    text-transform: $text-uppercase;
    padding: 8px 16px;
    position: absolute;
    bottom: -15px;
    left: 125px;
    display: inline-block;
    &:hover {
      cursor: pointer;
    }
  }
}

.container-cards {
  display: $d-flex;
  justify-content: center;
  flex-wrap: wrap;
  width: $w-80;
  padding-top: 10px;
}

.button {
  padding: 20px;

  .btn-load {
    color: $text-white;
    background-color: $azure-bg-color;
    border: none;
    padding: 6px 35px;
    text-transform: $text-uppercase;
    font-weight: $text-bold;
    font-size: $font-size-5;
    &:hover {
      cursor: pointer;
    }
  }
}
</style>