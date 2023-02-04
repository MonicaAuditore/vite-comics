<script>
import AppHeader from "./components/AppHeader.vue";
import AppSubHeader from "./components/AppSubHeader.vue";
import BONUS_AppUpMain from "./components/BONUS_AppUpMain.vue";
import AppMain from "./components/AppMain.vue";
import AppFooter from "./components/AppFooter.vue";
import AppCard from "./components/AppCard.vue";

export default {
  components: {
    AppHeader,

    AppSubHeader,
    AppCard,
    BONUS_AppUpMain,
    AppMain,
    AppFooter,
  },
  data() {
    return {};
  },
};
</script>

<template>
  <AppHeader />
  <AppSubHeader />
  <AppCard />
  <BONUS_AppUpMain />
  <AppMain />
  <AppFooter />
</template>

<style lang="scss">
@use "./styles/main.scss";
</style>
