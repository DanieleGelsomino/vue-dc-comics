<template>
  <footer>
    <!-- icone con link -->
    <div class="top-footer">
      <ul>
        <li>
          <img src="../assets/buy-comics-digital-comics.png" alt="dc-digital-comics">
          <a href="#">digital comics</a>
        </li>
        <li>
          <img src="../assets/buy-comics-merchandise.png" alt="dc-merchandise">
          <a href="#">dc merchandise</a>
        </li>
        <li>
          <img src="../assets/buy-comics-subscriptions.png" alt="dc-subscriptions">
          <a href="#">subscription</a>
        </li>
        <li>
          <img src="../assets/buy-comics-shop-locator.png" alt="dc-shop-locator">
          <a href="#">comic shop locator</a>
        </li>
        <li>
          <img class="icon-power" src="../assets/buy-dc-power-visa.svg" alt="dc-power-visa">
          <a href="#">dc power visa</a>
        </li>
        
      </ul>

    </div>
    <!-- link con dc logo grande -->
    <div class="main-footer"></div>
    <!-- button sign-up e icone social -->
    <div class="bottom-footer"></div>

  </footer>
</template>

<script>
export default {
name:'FooterComponent'
}
</script>

<style scoped lang="scss">
@import "../variables";

.top-footer {
  background-color: $azure-bg-color;
  display: $d-flex;
  justify-content: center;
  ul {
    list-style-type: $list-style;
    display: $d-flex;
    justify-content: space-around;
    align-items:center;
    padding: 30px 0px;
    width: 80%;

    li {
      font-size: $font-size-6;
      font-weight: $text-bold;
      text-transform: $text-uppercase;
      display: $d-flex;
      align-items:center;
     
      a {
        text-decoration: $no-decoration;
        color:$text-white;
         margin-left: 8px;
      }
    }

    img {
      height: 35px;
    }

    .icon-power {
      height: 25px;
    }
  }

}

.main-footer {
  background-image: url('../assets/footer-bg.jpg');
  height: 350px;
}

.bottom-footer {
  background-color:$bg-darkgray;
  height: 100px;
}

</style>