<template>
  <footer>
      <div class="footer-top">

        <div class="container">

         <div class="columns">
            <div class="column">
            <h4>Dc Comics</h4>
            <ul>
              <li><a href="#">Charaters</a></li>
              <li><a href="#">Comics</a></li>
              <li><a href="#">Movies</a></li>
              <li><a href="#">TV</a></li>
              <li><a href="#">Games</a></li>
              <li><a href="#">Videos</a></li>
              <li><a href="#">News</a></li>
            </ul>

             <h4>Shop</h4>
             <ul>
               <li><a href="#">Shop DC</a></li>
               <li><a href="#">Shop DC Collectibles</a></li>
             </ul>

          </div>

          <div class="column">
            <h4>Dc</h4>
            <ul>
              <li><a href="#">Terms Of Use</a></li>
              <li><a href="#">Privacy Policy (New)</a></li>
              <li><a href="#">Ad Choise</a></li>
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

          <div class="column">
            <h4>Sites</h4>
            <ul>
              <li><a href="#">DC</a></li>
              <li><a href="#">MAD Magazine</a></li>
              <li><a href="#">DC Kids</a></li>
              <li><a href="#">DC Universe</a></li>
              <li><a href="#">DC Power Visa</a></li>
            </ul>

          </div>
         </div>

        <div class="footer-logo">
          <img src="../assets/img/dc-logo-bg.png" alt="">
        </div>

        </div>

      </div>

      <div class="footer-bottom">

        <div class="container">

          <div class="sign-up">
            SIGN-UP NOW!
          </div>

          <div class="icons-section">
            <div class="icon-text">
              <h3>FOLLOW US</h3>
            </div>
          <div class="icons">

            <img src="../assets/img/footer-facebook.png" alt="facebook">
            <img src="../assets/img/footer-twitter.png" alt="twitter">
            <img src="../assets/img/footer-youtube.png" alt="youtube">
            <img src="../assets/img/footer-pinterest.png" alt="pinterest">
            <img src="../assets/img/footer-periscope.png" alt="periscope">

          </div>

          </div>
          
        </div>

      </div>

  </footer>
</template>

<script>
export default {
  name: 'FooterComponent'
}
</script>

<style lang="scss" scoped>

  @import '../assets/style/mixins';
  @import '../assets/style/vars';
  @import '../assets/style/global';
  @import '../assets/style/utils';

  footer{
    .footer-top{
      background-image: url(../assets/img/footer-bg.jpg);

      .container{
        height: 300px;
        padding: 30px 0;
        @include center();
        overflow: hidden;

        h4{
          color: #fff;
          text-transform: uppercase;
        }

         .footer-logo img{
           width: 450px;
      
         }
      }

      .columns{
        display: flex;
      }

      .column{

        margin-right: 30px;

        ul {
          padding: 10px 0;
        }

        ul li a {
          color: #959595;
          font-size: 12px;
          
        }
      }
    }

    .footer-bottom{
      background-color: #303030;

      .container{
        height: 100px;
        @include center();

        .sign-up{
          color: #fff;
          padding: 10px;
          border: 2px solid $primary-color;
          cursor: pointer;
        }

        .icons-section{
          display: flex;
          align-items: center;
          
          .icon-text{
            color: $primary-color;
          }

          .icons img{
            margin-left: 15px;
          }
        }
      }
    }
  }



</style>