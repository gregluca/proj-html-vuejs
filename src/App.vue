<script>
import AppFooter from './components/AppFooter.vue';
import AppHeader from './components/AppHeader.vue';
import Apphero from './components/AppHero.vue';
import AppBody from './components/AppBody.vue';

export default {
  components: { AppFooter, Apphero, AppHeader, AppBody },

  data() {
    return {
      elemHeader: ["HOME ","ABOUT","PRICES","COURSES","LOCATIONS","BLOGS"]
    };
  },
}
</script>
<template>

<AppHeader :elems="elemHeader" />
<Apphero />
<AppBody />
<AppFooter />
</template>

<style lang="scss">
@use"./style/general.scss";
@import "@fortawesome/fontawesome-free/css/all.css";
</style>