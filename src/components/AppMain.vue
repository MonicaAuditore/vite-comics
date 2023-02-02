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
          <ul>
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
          <h3>--> Content goes here</h3>
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

.container {
  height: 110px;
}

ul {
  line-height: 110px;
  list-style: none;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

li {
  color: #fff;
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 10px;
}

.icon {
  width: 40px;
}
</style>
