<template>
  <main>
    <div class="content-main">
      <h3>-- Contest goes here --</h3>
      <div class="banner"></div>
    </div>
  </main>
</template>

<script>
export default {
name:'MainComponent'
}
</script>

<style scoped lang="scss">
@import "../variables";

.content-main {
  display: $d-flex;
  justify-content: space-between;
  align-items:center;
  width: 80%;
  h3 {
    color: $text-white;
  }


}
</style>