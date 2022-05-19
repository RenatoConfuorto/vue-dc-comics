<template>
  <div class="footer-action">
    <div class="container">
      <div class="sign-up-section">
        <a href="#">Sign-up Now!</a>
      </div>

      <div class="socials">
        <h3>Follow us</h3>
        <ul>
          <li v-for="(item, index) in socials" :key="index">
            <a :href="item.url">
              <img :src="require('../assets/img/footer-' + item.img)" :alt="item.social">
            </a>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "AppFooterAction",
  data() {
    return{
      socials: [
        {
          social: 'Facebook',
          url: '#',
          img: 'facebook.png'
        },
        {
          social: 'Twitter',
          url: '#',
          img: 'twitter.png'
        },
        {
          social: 'YouTube',
          url: '#',
          img: 'youtube.png'
        },
        {
          social: 'Pinterest',
          url: '#',
          img: 'pinterest.png'
        },
        {
          social: 'Periscope',
          url: '#',
          img: 'periscope.png'
        },
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";
@import "../style/common.scss";

.footer-action{
  background-color: $primary-color;

  .container{
    display: flex;
    justify-content: space-between;
    align-items: center;
    
    padding: 1.5rem 0;

    .sign-up-section{
      a{
        padding: 0.3rem;
        text-decoration: none;
        text-transform: uppercase;
        border: 2px solid $brand-color;
        color: white;
      }
    }
    
    .socials{
      display: flex;
      align-items: center;

      h3{
        text-transform: uppercase;
        color: $brand-color;
        font-size: 1rem;
        margin-right: 10px;
      }

      ul{
        li{
          width: 1.5rem;
          height: auto;
          margin-right: 10px;
          display: inline-block;

          img{
            width: 100%;
          }
        }
      }
    }
  }
  
}

</style>