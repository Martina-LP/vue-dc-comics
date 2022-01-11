<template>
  <footer>
    <div class="footer-container">
      <div class="container">
        <div class="row">
          <div class="link">
            <div class="col">
              <h3>DC Comics</h3>
              <div class="list">
                <ul>
                  <li><a href="#">Characters</a></li>
                  <li><a href="#">Comics</a></li>
                  <li><a href="#">Movies</a></li>
                  <li><a href="#">TV</a></li>
                  <li><a href="#">Games</a></li>
                  <li><a href="#">Videos</a></li>
                  <li><a href="#">News</a></li>
                </ul>
              </div>
              <h3>Shop</h3>
              <div class="list">
                <ul>
                  <li><a href="#">Shop DC</a></li>
                  <li><a href="#">Shop DC Collectibles</a></li>
                </ul>
              </div>
            </div>
            <div class="col">
              <h3>DC</h3>
              <div class="list">
                <ul>
                  <li><a href="#">Terms of Use</a></li>
                  <li><a href="#">Privacy policy (New)</a></li>
                  <li><a href="#">Ad Choices</a></li>
                  <li><a href="#">Advertising</a></li>
                  <li><a href="#">Jobs</a></li>
                  <li><a href="#">Subscriptions</a></li>
                  <li><a href="#">Talent Workshops</a></li>
                  <li><a href="#">CPSC Certificates</a></li>
                  <li><a href="#">Ratings</a></li>
                  <li><a href="">Shop Help</a></li>
                  <li><a href="#">Contact Us</a></li>
                </ul>
              </div>
            </div>
            <div class="col">
              <h3>Sites</h3>
              <div class="list">
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
        </div>
        <div class="footer-banner">

        </div>
      </div>
    </div>
    <div class="footer-banner">
      <div class="container">
        <div class="row">

          <button>SIGN-UP NOW!</button>

          <div class="social">
            <a href="#">FOLLOW US</a>
            <img src="../assets/img/footer-facebook.png" alt="Facebook">
            <img src="../assets/img/footer-twitter.png" alt="Twitter">
            <img src="../assets/img/footer-youtube.png" alt="YouTube">
            <img src="../assets/img/footer-pinterest.png" alt="Pinterest">
            <img src="../assets/img/footer-periscope.png" alt="Periscope">
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'Footer'
}
</script>

<style scoped lang="scss">
@import '../style/variables'

footer {
  .footer-container {
    padding: 30px 0;
    background-image: url(../assets/img/dc-logo-bg.png) 68% no-repeat, url(../assets/img/footer-bg.jpg) no-repeat;
    background-size: 650px, cover;

    .link {
      display: flex;
      flex-direction: row;

      .col {
        width: 170px;

        h3 {
          color: white;
          margin: 20px 0;
          text-transform: uppercase;
        }

        .list {
          ul {
            list-style: none;

            li {
              margin: 5px 0;

              a {
                font-size: 12 px;
                text-decoration: none;
                color: #959595;

                &:hover {
                  color: white;
                }
              }
            }
          }
        }
      }
    }
  }

  .footer-banner {
    background-color: $secondary_color;

    .row {
      justify-content: space-between;

      button {
        border: 2px solid $primary_color;
        background-color: $secondary_color;
        color: white;
        padding: 12px;
        margin: 30px 0;
        font-size: 18px;
        cursor: pointer;
      }

      .social {
        display: flex;
        align-items: center;

        img {
          margin: 0 10px;
        }

        a {
          text-decoration: none;
          color: $primary_color;
          font-weight: 600;
          margin-right: 5px;
        }
      }
    }
  }
}
</style>