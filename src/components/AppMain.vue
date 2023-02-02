<script>
import { createAssignmentExpression } from "@vue/compiler-core";

export default {
  name: "AppMain",
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

  <div class="subMain">
    <img class="bk" :src="getImagePath(`../assets/img/${bkImage}`)" />
    <div class="mainContainer">
      <div class="textContent">
        <div class="columnLeft">
          <div class="columnUno">
            <div class="menuUno">
              <h3>DC COMICS</h3>
              <ul class="listaSubMain">
                <li>Characters</li>
                <li>Comics</li>
                <li>Movies</li>
                <li>TV</li>
                <li>Games</li>
                <li>Videos</li>
                <li>News</li>
              </ul>
            </div>
            <div class="menuDue">
              <h3>SHOP</h3>
              <ul class="listaSubMain">
                <li>Shop DC</li>
                <li>Shop DC Collectibles</li>
              </ul>
            </div>
          </div>
          <div class="columnDue">
            <div class="menuTre">
              <h3>DC</h3>
              <ul class="listaSubMain">
                <li>Term of use</li>
                <li>Privacy policy (New)</li>
                <li>Ad Choices</li>
                <li>Advertising</li>
                <li>Jobs</li>
                <li>Subscription</li>
                <li>CPSC Certificates</li>
                <li>Rating</li>
                <li>Shop Help</li>
                <li>Contact Us</li>
              </ul>
            </div>
          </div>
          <div class="columnTre">
            <div class="menuQuattro">
              <h3>SITES</h3>
              <ul class="listaSubMain">
                <li>DC</li>
                <li>MAD Magazine</li>
                <li>DC Kids</li>
                <li>DC Universe</li>
                <li>DC Power Visa</li>
              </ul>
            </div>
          </div>
        </div>
        <div class="columnRight">
          <div class="bigLogo">
            <img :src="getImagePath(`../assets/img/${bigLogo}`)" />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped></style>
