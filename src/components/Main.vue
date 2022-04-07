<template>
  <main>
    <div class="provisional-content">
      <DcCards v-for="(item, index) in comics" :key="index" :comics="item" />
    </div>
  </main>
</template>

<script>
import DcCards from "@/data/dc-comics";

export default {
  name: "MainComponent",
  props: {
    comics: Array,
  },
  components: {
    DcCards,
  },
};
</script>

<style scoped lang="scss">
@import "@/variables";

.provisional-content {
  display: $d-flex;
  justify-content: space-between;
  align-items: center;
  width: $w-80;
  h3 {
    color: $text-white;
  }
}
</style>