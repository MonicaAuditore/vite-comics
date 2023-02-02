<script>
import AppHeader from "./components/AppHeader.vue";
import AppSubHeader from "./components/AppSubHeader.vue";

export default {
  components: {
    AppHeader,
    AppSubHeader,
  },
  data() {
    return {};
  },
};
</script>

<template>
  <AppHeader />
  <AppSubHeader />
</template>

<style scoped>
h1 {
  color: green;
}
</style>
