<script>
import AppFooter from './components/AppFooter.vue';
import AppFreeLesson from './components/AppFreeLesson.vue';
import AppHeader from './components/AppHeader.vue';
import Apphero from './components/AppHero.vue';
import AppButton from './components/AppButton.vue'

export default {
  components: { AppFooter, Apphero, AppHeader, AppFreeLesson, AppButton },

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
<AppFreeLesson />
<h1>ciao utente</h1>
<AppFooter />
<AppButton />
</template>
<style lang="scss">
@use"./style/general.scss";

</style>