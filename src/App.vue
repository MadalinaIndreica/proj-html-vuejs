<script>
import AppFooter from './components/AppFooter.vue';
import AppHeader from "./components/AppHeader.vue";

export default  {
  data (){
    return {

    }
  },
  components : { AppHeader, AppFooter }
}

</script>

<template>
  <AppHeader>

  </AppHeader>
  <AppFooter></AppFooter>

</template>

<style lang="scss">
@use "./style/general.scss";
@import "@fortawesome/fontawesome-free/css/all.css";

</style>
