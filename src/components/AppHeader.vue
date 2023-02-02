<script>
import { createAssignmentExpression } from "@vue/compiler-core";

export default {
  data() {
    return {
      logo: "dc-logo.png",
    };
  },
  methods: {
    getImagePath: function (imgPath) {
      return new URL(imgPath, import.meta.url).href;
    },
  },
};
</script>

<template>
  <div class="header">
    <div class="container">
      <div class="logo">
        <img :src="getImagePath(`../assets/img/${logo}`)" />
      </div>
    </div>
  </div>
</template>

<style scoped>
.container {
  width: 1000px;
  margin: 0 auto;
}
</style>
