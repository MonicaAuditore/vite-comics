<script>
import AppHeader from "./components/AppHeader.vue";
import AppSubHeader from "./components/AppSubHeader.vue";
import AppMain from "./components/AppMain.vue";
import AppFooter from "./components/AppFooter.vue";

export default {
  components: {
    AppHeader,
    AppSubHeader,
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
  <AppMain />
  <AppFooter />
</template>

<style scoped>
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
  font-family: "Roboto", sans-serif;
}
</style>
