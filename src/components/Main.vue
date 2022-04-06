<template>
  <main>
    <div class="provisional-content">
      <h3>--&gt; Contest goes here &lt;--</h3>
    </div>
  </main>
</template>

<script>
export default {
  name: "MainComponent",
};
</script>

<style scoped lang="scss">
@import "../variables";

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