<script>
export default {
  data() {
    return {};
  },
};
</script>

<template>
  <div class="cards">
    <div class="mainContainer">
      <div class="containerCard">
        <div class="card">
          <div class="imgCard">
            <a :href="singleCard.thumb"><img :src="singleCard.thumb" /></a>
          </div>
          <div class="title-card">{{ singleCard.series }}</div>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped></style>
