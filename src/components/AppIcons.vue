<template>
  <div class="icons-container">
    <ul>
      <li v-for="(item, index) in icons" :key="index">
        <a :href="item.url">
          <img :src="require('../assets/img/buy-' + item.img)" :alt="item.text">
          <span>{{ item.text }}</span>
        </a>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return{
      icons: [
        {
          url: '#',
          img: 'comics-digital-comics.png',
          text: 'Digital Comics'
        },
        {
          url: '#',
          img: 'comics-merchandise.png',
          text: 'Dc Merchandise'
        },
        {
          url: '#',
          img: 'comics-subscriptions.png',
          text: 'Subscription'
        },
        {
          url: '#',
          img: 'comics-shop-locator.png',
          text: 'Comic shop locator'
        },
        {
          url: '#',
          img: 'dc-power-visa.svg',
          text: 'Dc power visa'
        },
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
  @import "../style/variables.scss";
  @import "../style/common.scss";

.icons-container{
  width: 100%;
  height: $app-icons-height;
  background-color: $brand-color;
  ul{
    height: 100%;
    display: flex;
    justify-content: center;
    align-items: center;

    li{
      height: 35%;
      margin: 0 1rem;

      a{
        color: white;

        img{
          height: 100%;
          vertical-align: middle;
          margin-right: 10px;
        }

        span{
          font-size: 0.7rem;
          text-transform: uppercase;
          vertical-align: middle;
        }
      }
    }
  }
}
</style>