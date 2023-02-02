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
  <div class="subHeader">
    <div class="mainContainer">
      <div class="container">
        <div class="textContent">
          <h3>--> Content goes here</h3>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.subHeader {
  background-color: black;
}
.mainContainer {
  width: 1444px;
  margin: 0 auto;
}

.container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 110px;
}

h3 {
  color: #fff;
}

.menu {
  line-height: 110px;
}
</style>
