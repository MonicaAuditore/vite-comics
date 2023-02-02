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
        <!-- hamburger menu -->
        <nav>
          <div class="navbar">
            <div class="logoNav"></div>
            <div class="containerNavUno nav-container">
              <input class="checkbox" type="checkbox" name="" id="" />
              <div class="hamburger-lines">
                <span class="line line1"></span>
                <span class="line line2"></span>
                <span class="line line3"></span>
              </div>

              <!-- <div class="menu-items">
                <li><a href="#">CHARACTERS</a></li>
                <li><a href="#">COMICS</a></li>
                <li><a href="#">MOVIES</a></li>
                <li><a href="#">TV</a></li>
                <li><a href="#">GAMES</a></li>
                <li><a href="#">COLLECTIBLES</a></li>
                <li><a href="#">VIDEOS</a></li>
                <li><a href="#">FANS</a></li>
                <li><a href="#">NEWS</a></li>
                <li><a href="#">SHOP</a></li>
              </div> -->
            </div>
          </div>
        </nav>
        <!-- fine -->
      </div>
    </div>
  </div>
</template>

<style scoped></style>
