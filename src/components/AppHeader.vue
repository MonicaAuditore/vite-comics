<script>
import { createAssignmentExpression } from "@vue/compiler-core";

export default {
  name: "AppHeader",
  data() {
    return {
      name: "AppHeader",
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

<style scoped></style>
