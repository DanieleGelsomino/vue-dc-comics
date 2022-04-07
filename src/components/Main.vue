<template>
  <main>
    <div class="container-cards">
      <Cards
        v-for="(item, index) in comics"
        :key="'comic-' + index"
        :titleSeries="item.series"
        :urlImg="item.thumb"
      />
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

main {
  .container-cards {
    display: $d-flex;
    flex-wrap: wrap;
    width: $w-80;
  }
}
</style>