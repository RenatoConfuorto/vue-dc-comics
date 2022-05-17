<template>
  <div class="header">
    <div class="container">
      <div class="logo-wrapper">
        <img class="logo" src="../assets/img/dc-logo.png" alt="Dc Logo">
      </div>
      <nav class="nav-bar">
        <ul>
          <li v-for="(item, index) in navItems" :key="index">
            <a :href="item.url">{{ item.text }}</a>

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
      navItems:[
        {
          text: 'characters',
          url: '#',
          active: false
        },
        {
          text: 'comics',
          url: '#',
          active: false
        },
        {
          text: 'movies',
          url: '#',
          active: false
        },
        {
          text: 'tv',
          url: '#',
          active: false
        },
        {
          text: 'games',
          url: '#',
          active: false
        },
        {
          text: 'collectibles',
          url: '#',
          active: false
        },
        {
          text: 'videos',
          url: '#',
          active: false
        },
        {
          text: 'fans',
          url: '#',
          active: false
        },
        {
          text: 'news',
          url: '#',
          active: false
        },
        {
          text: 'shop',
          url: '#',
          active: false
        },
      ]
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
        height: 80%;
  
        .logo{
          height: 100%;
        }
  
      }
  
      .nav-bar{
  
        li{
          padding: 0.5rem;
          display: inline-block;
          text-transform: uppercase;
          font-size: 0.75rem;
          font-weight: 500;
        }
      }

    }

  }

</style>