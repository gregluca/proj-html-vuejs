<script>
import AppFooter from './components/AppFooter.vue';
import AppHeader from './components/AppHeader.vue';
import Apphero from './components/AppHero.vue';

export default {
  components: { AppFooter, Apphero, AppHeader },

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
<h1>ciao utente</h1>
<AppFooter />

</template>
<style lang="scss">
@use"./style/general.scss";

</style>