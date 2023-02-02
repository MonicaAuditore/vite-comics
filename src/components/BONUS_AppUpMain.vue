<script>
import { createAssignmentExpression } from "@vue/compiler-core";

export default {
  name: "AppUpMain",
  data() {
    return {
      iconUno: "buy-comics-digital-comics.png",
      iconDue: "buy-comics-merchandise.png",
      iconTre: "buy-comics-subscriptions.png",
      iconQuattro: "buy-comics-shop-locator.png",
      iconCinque: "buy-dc-power-visa.svg",
      bkImage: "footer-bg.jpg",
      bigLogo: "dc-logo-bg.png",
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
  <div class="main">
    <div class="mainContainer">
      <div class="container">
        <div class="textContentBlu">
          <ul class="listaBlu">
            <li>
              <img
                class="icon"
                :src="getImagePath(`../assets/img/${iconUno}`)"
              /><span>DIGITAL COMICS</span>
            </li>
            <li>
              <img
                class="icon"
                :src="getImagePath(`../assets/img/${iconDue}`)"
              /><span>DC MERCHANDAISE</span>
            </li>
            <li>
              <img
                class="icon"
                :src="getImagePath(`../assets/img/${iconTre}`)"
              /><span>SUBSCRIPTION</span>
            </li>
            <li>
              <img
                class="icon"
                :src="getImagePath(`../assets/img/${iconQuattro}`)"
              /><span>COMIC SHOP LOCATOR</span>
            </li>
            <li>
              <img
                class="icon"
                :src="getImagePath(`../assets/img/${iconCinque}`)"
              /><span>DC POWER VISA</span>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped></style>
