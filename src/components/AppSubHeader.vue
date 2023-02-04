<script>
import { createAssignmentExpression } from "@vue/compiler-core";

export default {
  name: "AppSubHeader",
  data() {
    return {};
  },
  methods: {
    getImagePath: function (imgPath) {
      return new URL(imgPath, import.meta.url).href;
    },
  },
};
</script>

<template>
  <div class="subHeader"></div>
</template>

<style scoped></style>
