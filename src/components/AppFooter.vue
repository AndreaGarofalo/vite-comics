<script>
export default {
  name: "DC Footer",
};
</script>

<template>
  <footer>
    <div class="container">
      <div class="footer-row">
        <div class="footer-col">
          <h3>DC COMICS</h3>
          <ul>
            <li><a href="#"> Characters</a></li>
            <li><a href="#">Comics</a></li>
            <li><a href="#">Movie</a></li>
            <li><a href="#">TV</a></li>
            <li><a href="#">Games</a></li>
            <li><a href="#">Videos</a></li>
            <li><a href="#">News</a></li>
          </ul>
          <h3>SHOP</h3>
          <ul>
            <li><a href="#">Shop DC</a></li>
            <li><a href="#">Shop DC Collectibles</a></li>
          </ul>
        </div>
        <div class="footer-col">
          <h3>DC</h3>
          <ul>
            <li><a href="#">Terms Of Use</a></li>
            <li><a href="#">Privacy policy (New)</a></li>
            <li><a href="#">Ad Choices</a></li>
            <li><a href="#">Advertising</a></li>
            <li><a href="#">Jobs</a></li>
            <li><a href="#">Subscriptions</a></li>
            <li><a href="#">Talent Workshops</a></li>
            <li><a href="#">CPSC Certificates</a></li>
            <li><a href="#">Ratings</a></li>
            <li><a href="#">Shop Help</a></li>
            <li><a href="#">Contact us</a></li>
          </ul>
        </div>
        <div class="footer-col">
          <h3>SITES</h3>
          <ul>
            <li><a href="#">DC</a></li>
            <li><a href="#">MAD Magazine</a></li>
            <li><a href="#">DC Kids</a></li>
            <li><a href="#">DC Universe</a></li>
            <li><a href="#">DC Power Visa</a></li>
          </ul>
        </div>
      </div>
    </div>
  </footer>

  <section class="follow-link">
    <div class="container">
      <a href="#" class="sign-up">SIGN-UP NOW</a>
      <div class="our-socials">
        <h2>Follow Us</h2>
        <a href=""
          ><img src="../assets/img/footer-facebook.png" alt="facebook"
        /></a>
        <a href=""
          ><img src="../assets/img/footer-youtube.png" alt="facebook"
        /></a>
        <a href=""
          ><img src="../assets/img/footer-twitter.png" alt="facebook"
        /></a>
        <a href=""
          ><img src="../assets/img/footer-pinterest.png" alt="facebook"
        /></a>
        <a href=""
          ><img src="../assets/img/footer-periscope.png" alt="facebook"
        /></a>
      </div>
    </div>
  </section>
</template>

<style scoped lang="scss">
@use "../assets/scss/partials/variables" as *;
footer {
  .container {
    max-width: 1200px;
    margin: 0 auto;
    background-image: url("../assets/img/dc-logo-bg.png");
    background-position: right;
    background-repeat: no-repeat;
    .footer-row {
      display: flex;
      justify-content: flex-start;
      .footer-col {
        padding: 2rem 1rem;
        h3 {
          padding: 15px 0;
          color: $white;
        }
        li {
          list-style-type: none;
          color: $gray;
          a {
            font-size: 12px;
            display: inline-block;
            padding: 3px 0;
            color: $gray;
          }
        }
      }
    }
  }
}
.follow-link {
  height: 6rem;
  background-color: #303030;
  .container {
    height: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    .sign-up {
      border: 2px solid $blue;
      color: $blue;
      padding: 5px 10px;
    }
    .our-socials {
      display: flex;
      align-items: center;
      h2 {
        color: $blue;
        padding: 0 1rem;
      }
      img {
        color: $gray;
        font-size: 16px;
        padding: 0 5px;
      }
    }
  }
}
</style>
