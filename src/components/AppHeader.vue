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
    <div class="mainContainer">
      <div class="container">
        <div class="logo">
          <img :src="getImagePath(`../assets/img/${logo}`)" />
        </div>
        <div class="menu">
          <ul>
            <li>CHARACTERS</li>
            <li>COMICS</li>
            <li>MOVIES</li>
            <li>TV</li>
            <li>GAMES</li>
            <li>COLLECTIBLES</li>
            <li>VIDEOS</li>
            <li>FANS</li>
            <li>NEWS</li>
            <li>SHOP</li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
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

.menu {
  line-height: 110px;
}

.menu ul {
  display: flex;
}

.menu ul li {
  list-style: none;
  padding: 0px 10px;
}

.menu ul li:hover {
  box-shadow: inset 0em -0.3em #0282f9;
}
</style>
