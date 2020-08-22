<template>
    <div class="home">
      <header class="g-header-container">
        <home-header/>
      </header>
      <me-scroll>
        <home-slide/>
        <home-nav/>
        <home-recommend/>
      </me-scroll>
      <div class="g-backtop-container"></div>
      <router-view></router-view>
    </div>
</template>

<script>
  import HomeHeader from './header';
  import HomeSlide from './slider';
  import MeScroll from 'base/scroll';
  import HomeNav from './nav';
  import HomeRecommend from './recommend';

  export default {

    name: 'Home',

    components: {
      HomeRecommend,
      HomeNav,
      HomeHeader,
      HomeSlide,
      MeScroll
    }

  };

  // console.log(document.body.offsetHeight);
</script>

<style lang="scss" scoped>
@import "~assets/scss/mixins";
  .home {
  overflow:hidden;
  width:100%;
  height:100%;
  background-color: $bgc-theme;
  }
</style>
