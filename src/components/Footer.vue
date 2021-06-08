<template>
  <div>
      <div id="footer">
        <div class="container">
            <div id="links">
                <div id="col-1">
                    <div>
                        <h2>DC COMICS</h2>
                        <ul>
                            <li>Charatecters</li>
                            <li>Comics</li>
                            <li>Mobies</li>
                            <li>TV</li>
                            <li>Games</li>
                            <li>Videos</li>
                            <li>News</li>
                        </ul>
                    </div>

                    <div>
                        <h2>SHOP</h2>
                        <ul>
                            <li>Shop DC</li>
                            <li>Shop DC Collectibles</li>
                        </ul>
                    </div>
                </div>

                <div id="col-2">
                    <h2>DC</h2>
                    <ul>
                        <li>Terms Of Use</li>
                        <li>Privacy policy (New)</li>
                        <li>Ad Choices</li>
                        <li>Advertising</li>
                        <li>Jobs</li>
                        <li>Subscriptions</li>
                        <li>Talent Workshops</li>
                        <li>CPSC Certificates</li>
                        <li>Ratings</li>
                        <li>Shop Helps</li>
                        <li>Contact Us</li>
                    </ul>
                </div>

                <div id="col-3">
                    <h2>SITES</h2>
                    <ul>
                        <li>DC</li>
                        <li>MAD Magazine</li>
                        <li>DC Kids</li>
                        <li>DC Universe</li>
                        <li>DC Power Visa</li>
                    </ul>
                </div>
            </div>
            <img id="logo-footer" src="../assets/img/dc-logo-bg.png" alt="logo">
        </div>
      </div>
      <nav>
          <div class="container">
              <div>
                  <h4>SIGN-UP NOW!</h4>
              </div>
              <div id="icons">
                  <h3>FOLLOW US</h3>
                  <ul>
                      <li>
                          <img src="../assets/img/footer-facebook.png" alt="facebook">
                      </li>
                      <li>
                          <img src="../assets/img/footer-twitter.png" alt="twitter">
                      </li>
                      <li>
                          <img src="../assets/img/footer-youtube.png" alt="youtube">
                      </li>
                      <li>
                          <img src="../assets/img/footer-pinterest.png" alt="pinterest">
                      </li>
                      <li>
                          <img src="../assets/img/footer-periscope.png" alt="periscope">
                      </li>
                  </ul>
              </div>
          </div>
      </nav>
  </div>
</template>

<script>
export default {
    name: "Footer",
}
</script>

<style lang="scss" scoped>

    $colorBlue : #0282F9;

    #footer {
        background: url("../assets/img/footer-bg.jpg") no-repeat;
        background-size: cover;
        color: white;
        padding: 40px;
        overflow: hidden;
    }
    #logo-footer {
        position: absolute;
        top: -48%;
        right: 0;
    }
    h2 {
        font-size: 20px;
        margin: 20px 0;
    }
    ul {
        list-style: none;

        li {
            opacity: 0.5;
            margin: 5px 0;
            font-size: 12px;

            &:hover {
                text-decoration: underline;
                cursor: pointer;
            }
        }
    }
    .container {
        position: relative;
    }

    #links {
        display: flex;

        & > * {
            padding: 0 15px;
        }
    }

    nav {
        padding: 30px 0;
        background-color: #303030;

        h3 {
            color: $colorBlue;
            margin-right: 20px;
            cursor: pointer;
        }

        li {
            display: inline-block;
            margin: 0 10px;

            &:hover {
                filter: brightness(100);
            }
        }
        .container{
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        #icons {
            display: flex;
            align-items: center;
        }

        h4 {
            color: white;
            padding: 10px;
            border: 2px solid $colorBlue;
        }
    }
</style>