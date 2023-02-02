<script>
import { createAssignmentExpression } from "@vue/compiler-core";

export default {
  name: "AppFooter",
  data() {
    return {
      iconFacebook: "footer-facebook.png",
      iconTwitter: "footer-twitter.png",
      iconYoutube: "footer-youtube.png",
      iconPinterest: "footer-pinterest.png",
      iconLocator: "footer-periscope.png",
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
  <div class="footer">
    <div class="mainContainer">
      <div class="container">
        <div class="footerLeft">
          <div class="button">
            <a href="#">SIGN-UP NOW!</a>
          </div>
        </div>
        <div class="footerRight">
          <ul class="follow">
            <li><span class="followText">FOLLOW US</span></li>
            <li>
              <a href="#"
                ><img :src="getImagePath(`../assets/img/${iconFacebook}`)"
              /></a>
            </li>
            <li>
              <a href="#"
                ><img :src="getImagePath(`../assets/img/${iconTwitter}`)"
              /></a>
            </li>
            <li>
              <a href="#"
                ><img :src="getImagePath(`../assets/img/${iconYoutube}`)"
              /></a>
            </li>
            <li>
              <a href="#">
                <img :src="getImagePath(`../assets/img/${iconPinterest}`)"
              /></a>
            </li>
            <li>
              <a href="#"
                ><img :src="getImagePath(`../assets/img/${iconLocator}`)"
              /></a>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.mainContainer {
  width: 1444px;
  margin: 0 auto;
}

.footer {
  background-color: #303030;
  height: 110px;
  display: flex;

  align-items: center;
}

.container {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.button a {
  text-decoration: none;
  color: #fff;
  padding: 15px;
  border: 2px solid #0282f9;
}

.followText {
  font-weight: bold;
  color: #0282f9;
  font-size: 21px;
}

.follow {
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: 18px;
  list-style: none;
}
</style>
