<template>
  <footer>
    <!-- icone con link -->
    <div class="top-footer">
      <ul>
        <li>
          <img
            src="../assets/buy-comics-digital-comics.png"
            alt="dc-digital-comics"
          />
          <a href="#">digital comics</a>
        </li>
        <li>
          <img
            src="../assets/buy-comics-merchandise.png"
            alt="dc-merchandise"
          />
          <a href="#">dc merchandise</a>
        </li>
        <li>
          <img
            src="../assets/buy-comics-subscriptions.png"
            alt="dc-subscriptions"
          />
          <a href="#">subscription</a>
        </li>
        <li>
          <img
            src="../assets/buy-comics-shop-locator.png"
            alt="dc-shop-locator"
          />
          <a href="#">comic shop locator</a>
        </li>
        <li>
          <img
            class="icon-power"
            src="../assets/buy-dc-power-visa.svg"
            alt="dc-power-visa"
          />
          <a href="#">dc power visa</a>
        </li>
      </ul>
    </div>
    <!-- link con dc logo grande -->
    <div class="main-footer">
      <div class="link-list">
        <div class="link-image">
          <ul>
            <h3>dc comics</h3>
            <li><a href="#">Characters</a></li>
            <li><a href="#">Comics</a></li>
            <li><a href="#">Movies</a></li>
            <li><a href="#">Tv</a></li>
            <li><a href="#">Games</a></li>
            <li><a href="#">Videos</a></li>
            <li><a href="#">News</a></li>
          </ul>
          <ul>
            <h3>dc</h3>
            <li><a href="#">Terms Of Use</a></li>
            <li><a href="#">Privacy policy(new)</a></li>
            <li><a href="#">Ad Choices</a></li>
            <li><a href="#">Advertising</a></li>
            <li><a href="#">Subsciptions</a></li>
            <li><a href="#">Talent Workshops</a></li>
            <li><a href="#">CPSC Certificates</a></li>
            <li><a href="#">Ratings</a></li>
            <li><a href="#">shop Help</a></li>
            <li><a href="#">contact Us</a></li>
          </ul>
          <ul>
            <h3>sites</h3>
            <li><a href="#">DC</a></li>
            <li><a href="#">MAD Magazine</a></li>
            <li><a href="#">DC Kids</a></li>
            <li><a href="#">DC Universe</a></li>
            <li><a href="#">DC Power Visa</a></li>
          </ul>
          <ul>
            <h3>shop</h3>
            <li><a href="#">Shop DC</a></li>
            <li><a href="#">Shop DC Collectibles</a></li>
          </ul>
        </div>
      </div>
    </div>
    <!-- button sign-up e icone social -->
    <div class="bottom-footer">
      <div class="connect">
        <button class="btn">Sign-up now</button>

        <div class="icons">
          <h3>Follow us</h3>
          <img src="../assets/footer-facebook.png" alt="facebook" />
          <img src="../assets/footer-twitter.png" alt="twitter" />
          <img src="../assets/footer-youtube.png" alt="youtube" />
          <img src="../assets/footer-pinterest.png" alt="pinterest" />
          <img src="../assets/footer-periscope.png" alt="periscope" />
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "FooterComponent",
};
</script>

<style scoped lang="scss">
@import "@/variables";

.top-footer {
  background-color: $azure-bg-color;
  display: $d-flex;
  justify-content: center;
  ul {
    list-style-type: $list-style;
    display: $d-flex;
    flex-wrap: wrap;
    justify-content: space-around;
    align-items: center;
    padding: 30px 0px;
    width: $w-80;

    li {
      font-size: $font-size-6;
      font-weight: $text-bold;
      text-transform: $text-uppercase;
      display: $d-flex;
      align-items: center;

      a {
        text-decoration: $no-decoration;
        color: $text-white;
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
  background-image: url("../assets/footer-bg.jpg");
  background-size: 380px, cover;
  display: $d-flex;
  justify-content: center;

  .link-list {
    background-image: url("../assets/dc-logo-bg.png");
    background-repeat: no-repeat;
    background-size: 380px;
    background-position: right;
    display: $d-flex;
    flex-wrap: wrap;
    width: $w-80;
    color: $text-white;
    h3 {
      text-transform: $text-uppercase;
      font-size: $font-size-8;
    }
    .link-image {
      display: $d-flex;
      flex-wrap: wrap;
      padding: 20px 0px;
    }
    ul {
      list-style-type: $list-style;
      display: $d-flex;
      flex-direction: $f-direction-column;
      align-items: flex-start;
      width: 30%;

      li {
        line-height: 12px;
      }

      a {
        color: $text-ligthgray;
        text-decoration: $no-decoration;
        font-size: $font-size-6;
        font-weight: $text-bold;
        &:hover {
          color: $text-azure;
          text-decoration: underline;
        }
      }
    }
  }
}

.bottom-footer {
  background-color: $bg-darkgray;
  display: $d-flex;
  justify-content: center;

  .connect {
    display: $d-flex;
    justify-content: space-between;
    width: $w-80;
    padding: 30px 0px;

    .btn {
      background-color: $bg-darkgray;
      border: 2px solid $azure-bg-color;
      color: $text-white;
      text-transform: $text-uppercase;
      font-weight: $text-bold;
      font-size: $font-size-6;
      padding: 8px 10px;
      &:hover {
        cursor: pointer;
      }
    }

    .icons {
      display: $d-flex;
      align-items: center;
      padding: 5px;
      h3 {
        color: $text-azure;
        text-transform: $text-uppercase;
        font-size: $font-size-9;
        margin-right: 8px;
      }

      img {
        width: 25px;
        margin-left: 8px;
        &:hover {
          cursor: pointer;
        }
      }
    }
  }
}
</style>