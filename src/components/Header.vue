<template>
  <header>
    <div class="container">
      <div class="header-wrapper">
        <!-- Logo -->
        <div class="logo">
          <img src="../assets/img/dc-logo.png" alt="DC Logo">
        </div>
        <!-- Nav -->
        <nav>
          <ul class="menu">
            <li v-for="(link, index) in links" :key="index">
              <a :href="link.url" :class="{ 'current': link.current }">{{ link.text }}</a>
            </li>
          </ul>
        </nav>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: "Header",

  data: function() {
    return {
      links: [
        {
          text: 'Characters',
          url: '#',
          current: false,
        },
        {
          text: 'Comics',
          url: '#',
          current: true,
        },
        {
          text: 'Movies',
          url: '#',
          current: false,
        },
        {
          text: 'TV',
          url: '#',
          current: false,
        },
        {
          text: 'Games',
          url: '#',
          current: false,
        },
        {
          text: 'Collectibles',
          url: '#',
          current: false,
        },
        {
          text: 'Videos',
          url: '#',
          current: false,
        },
        {
          text: 'Fans',
          url: '#',
          current: false,
        },
        {
          text: 'News',
          url: '#',
          current: false,
        },
        {
          text: 'Shop',
          url: '#',
          current: false,
        },
      ]
    }
  }
  
}
</script>

<style scoped lang="scss">
@import '../style/variables.scss';

header {

  .header-wrapper {
    display: flex;
    height: 120px;
    justify-content: space-between;
    align-items: center;

    .logo {
      
      img {
        width: 60px;

      }
    }

    .menu {
      display: flex;

      li {
        margin-left: 10px;

        a {
          display: inline-block;
          color: inherit;
          font-size: 18px;
          text-decoration: none;
          text-transform: uppercase;
          font-weight: bold;
          line-height: 120px;

          &.current {
            color: $primary_color;
            border-bottom: 4px solid $primary_color;
            line-height: 116px;
          }

        }
      }
    }
  }

  
}

</style>
