<template>
  <div class="header">
    <div class="container">
      <div class="logo-wrapper">
        <img class="logo" src="../assets/img/dc-logo.png" alt="Dc Logo">
      </div>
      <nav class="nav-bar">
        <ul>
          <li v-for="(item, index) in navItems" :class="{'active': activeItem == index}" :key="index">
            <a :href="item.url" @click="changeActive(index)">{{ item.text }}</a>

          </li>
        </ul>
      </nav>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return{
      activeItem: 1,
      navItems:[
        {
          text: 'characters',
          url: '#',
        },
        {
          text: 'comics',
          url: '#',
        },
        {
          text: 'movies',
          url: '#',
        },
        {
          text: 'tv',
          url: '#',
        },
        {
          text: 'games',
          url: '#',
        },
        {
          text: 'collectibles',
          url: '#',
        },
        {
          text: 'videos',
          url: '#',
        },
        {
          text: 'fans',
          url: '#',
        },
        {
          text: 'news',
          url: '#',
        },
        {
          text: 'shop',
          url: '#',
        },
      ]
    }
  },
  methods: {
    changeActive(index){
      this.activeItem = index;
    }
  }
}
</script>

<style lang="scss" scoped>
  @import "../style/variables.scss";
  @import "../style/common.scss";

  .header{
    background-color: white;
    height: $header-height;
    width: 100%;

    .container{

      display: flex;
      justify-content: space-between;
      align-items: center;

      .logo-wrapper{
        height: 75%;
  
        .logo{
          height: 100%;
        }
  
      }
  
      .nav-bar{
        height: 100%;
  
        li{
          height: $header-height;
          margin: 0 0.5rem;
          display: inline-block;
          text-transform: uppercase;
          font-size: 0.8rem;
          font-weight: 500;
          line-height: $header-height;

          &.active{
            border-bottom: 3px solid $brand-color;

            a{
              color: $brand-color;
            }
          }
        }
      }

    }

  }

</style>