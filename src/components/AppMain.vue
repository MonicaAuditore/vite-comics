<script>
import { createAssignmentExpression } from "@vue/compiler-core";

export default {
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
    <div class="mainContainer">
      <div class="container">
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
                <h3>DC COMICS</h3>
                <ul class="listaSubMain">
                  <li>Characters</li>
                  <li>Comics</li>
                </ul>
              </div>
            </div>
            <div class="columnDue">
              <div class="menuTre">
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
            </div>
            <div class="columnTre">
              <div class="menuQuattro">
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
  </div>
</template>

<style scoped>
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
.main {
  background-color: #0282f9;
}
.mainContainer {
  width: 1444px;
  margin: 0 auto;
}

.textContent {
  display: flex;
  justify-content: space-between;
}

.listaBlu {
  line-height: 110px;
  list-style: none;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.listaBlu li {
  color: #fff;
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 10px;
  cursor: pointer;
}

.icon {
  width: 40px;
}

.subMain {
  background-color: rgb(43, 43, 43);
  height: 455px;
  overflow: hidden;
  display: flex;
  padding: 30px 0px;
  position: relative;
}

h3 {
  color: #fff;
  padding: 20px 0px;
}

.listaSubMain {
  list-style: none;
  color: #fff;
}

.listaSubMain li {
  padding: 5px 0px;
}

.columnLeft {
  display: flex;
  gap: 72px;
}

.columnRight img {
  position: absolute;
  top: -63px;
  right: 273px;
}
</style>
