<script>
import AppFooter from './components/AppFooter.vue';
import AppHeader from "./components/AppHeader.vue";
import AppMain from "./components/AppMain.vue"

export default  {
  data (){
    return {
      headerNav: [
        'Home',
        'Shop',
        'Products',
        'Categories',
        'News',
        'Elements'
      ]

    }
  },
  components : { AppHeader, AppFooter, AppMain}
}

</script>

<template>
  <AppHeader :navItems="headerNav"></AppHeader>
  <AppMain/>
  <AppFooter></AppFooter>

</template>

<style lang="scss">
@use "./style/general.scss";
@import "@fortawesome/fontawesome-free/css/all.css";

</style>
