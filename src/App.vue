<script>
import AppHeader from "./components/AppHeader.vue";
import AppSubHeader from "./components/AppSubHeader.vue";
import AppMain from "./components/AppMain.vue";

export default {
  components: {
    AppHeader,
    AppSubHeader,
    AppMain,
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
</template>

<style scoped>
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
</style>
