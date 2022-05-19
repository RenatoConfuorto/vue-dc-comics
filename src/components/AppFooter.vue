<template>
  <div class="footer">
    <div class="container">
      <div class="footer-list">

        <div class="col-3">
          <h3>Dc Comics</h3>
          <ul>
            <li><a href="#">Characters</a></li>
            <li><a href="#">Comics</a></li>
            <li><a href="#">Movies</a></li>
            <li><a href="#">Tv</a></li>
            <li><a href="#">Games</a></li>
            <li><a href="#">Videos</a></li>
            <li><a href="#">News</a></li>
          </ul>


          <h3>Shop</h3>
          <ul>
            <li><a href="#">Shop Dc</a></li>
            <li><a href="#">Shop Dc Collectibles</a></li>
          </ul>
        </div>

        <div class="col-3">
          <h3>Dc</h3>
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
            <li><a href="#">Contact Us</a></li>
          </ul>

        </div>

        <div class="col-3">
          <h3>Sites</h3>
          <ul>
            <li><a href="#">DC</a></li>
            <li><a href="#">MAD Magazines</a></li>
            <li><a href="#">DC Kids</a></li>
            <li><a href="#">DC Universe</a></li>
            <li><a href="#">DC Power Visa</a></li>

          </ul>
        </div>

        
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "AppFooter",
  
}
</script>

<style lang="scss" scoped>
  @import "../style/variables.scss";
  @import "../style/common.scss";

  .footer{
    background-image: url('../assets/img/footer-bg.jpg');
    
    .container{
      padding: 2rem 0 1rem;
      background-image: url('../assets/img/dc-logo-bg.png');
      background-position: right;
      background-repeat: no-repeat;
      background-size: 50% auto;

      .footer-list{
        width: 50%;
        height: 100%;
        display: flex;

        .col-3{
          flex-basis: calc(100% / 3);
          color: white;

          h3{
            text-transform: uppercase;
            margin-bottom: 1rem;
          }

          ul{
            margin-bottom: 1rem;

            li{
              margin-bottom: 5px;
              font-size: 0.8rem;
              a{
                color: #8e8e90;
              }
            }
          }
        }
      }
    }
  }
</style>